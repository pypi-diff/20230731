# Comparing `tmp/dydxpy-0.3.0.post1.tar.gz` & `tmp/dydxpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dydxpy-0.3.0.post1.tar", max compression
+gzip compressed data, was "dydxpy-0.3.1.tar", max compression
```

## Comparing `dydxpy-0.3.0.post1.tar` & `dydxpy-0.3.1.tar`

### file list

```diff
@@ -1,648 +1,648 @@
--rw-r--r--   0        0        0     1405 2023-07-17 13:45:23.246073 dydxpy-0.3.0.post1/LICENSE
--rw-r--r--   0        0        0     1938 2023-07-31 20:12:02.189987 dydxpy-0.3.0.post1/README.md
--rw-r--r--   0        0        0        0 2023-06-29 20:38:48.782587 dydxpy-0.3.0.post1/dydxpy/__init__.py
--rw-r--r--   0        0        0       85 2023-07-31 20:03:17.669681 dydxpy-0.3.0.post1/dydxpy/proto/__init__.py
--rw-r--r--   0        0        0     1977 2023-07-31 20:04:37.339547 dydxpy-0.3.0.post1/dydxpy/proto/amino/amino_pb2.py
--rw-r--r--   0        0        0      601 2023-07-31 20:04:37.339691 dydxpy-0.3.0.post1/dydxpy/proto/amino/amino_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.340662 dydxpy-0.3.0.post1/dydxpy/proto/amino/amino_pb2_grpc.py
--rw-r--r--   0        0        0     1964 2023-07-31 20:04:37.341030 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/runtime/v1alpha1/module_pb2.py
--rw-r--r--   0        0        0     1860 2023-07-31 20:04:37.341134 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.341213 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/runtime/v1alpha1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1798 2023-07-31 20:04:37.341326 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/config_pb2.py
--rw-r--r--   0        0        0     1769 2023-07-31 20:04:37.341404 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.341606 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/config_pb2_grpc.py
--rw-r--r--   0        0        0     1961 2023-07-31 20:04:37.341744 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/module_pb2.py
--rw-r--r--   0        0        0     1597 2023-07-31 20:04:37.341849 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.341926 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1613 2023-07-31 20:04:37.342092 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2.py
--rw-r--r--   0        0        0      645 2023-07-31 20:04:37.342465 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2.pyi
--rw-r--r--   0        0        0     2603 2023-07-31 20:04:37.342624 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1763 2023-07-31 20:04:37.342845 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1368 2023-07-31 20:04:37.342924 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.342995 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4477 2023-07-31 20:04:37.343140 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/auth_pb2.py
--rw-r--r--   0        0        0     2825 2023-07-31 20:04:37.343232 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.343308 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/auth_pb2_grpc.py
--rw-r--r--   0        0        0     1902 2023-07-31 20:04:37.343387 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      946 2023-07-31 20:04:37.343478 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.343544 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    12687 2023-07-31 20:04:37.343641 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     5358 2023-07-31 20:04:37.343731 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    19125 2023-07-31 20:04:37.344000 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2878 2023-07-31 20:04:37.344268 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0      929 2023-07-31 20:04:37.344491 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2743 2023-07-31 20:04:37.344626 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1338 2023-07-31 20:04:37.344836 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/module/v1/module_pb2.py
--rw-r--r--   0        0        0      329 2023-07-31 20:04:37.345023 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.345131 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4042 2023-07-31 20:04:37.345297 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     2077 2023-07-31 20:04:37.345384 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.345456 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0     2375 2023-07-31 20:04:37.345540 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/event_pb2.py
--rw-r--r--   0        0        0     1078 2023-07-31 20:04:37.345606 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.345667 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/event_pb2_grpc.py
--rw-r--r--   0        0        0     1747 2023-07-31 20:04:37.345739 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      815 2023-07-31 20:04:37.345820 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.345878 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     5552 2023-07-31 20:04:37.346012 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     3422 2023-07-31 20:04:37.346120 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6331 2023-07-31 20:04:37.346219 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     5201 2023-07-31 20:04:37.346331 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2267 2023-07-31 20:04:37.346413 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     6246 2023-07-31 20:04:37.346559 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3978 2023-07-31 20:04:37.346713 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/options_pb2.py
--rw-r--r--   0        0        0     4987 2023-07-31 20:04:37.346798 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/options_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.346864 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/options_pb2_grpc.py
--rw-r--r--   0        0        0     2467 2023-07-31 20:04:37.346958 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/query_pb2.py
--rw-r--r--   0        0        0     1197 2023-07-31 20:04:37.347015 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2886 2023-07-31 20:04:37.347073 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1426 2023-07-31 20:04:37.347223 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/module/v1/module_pb2.py
--rw-r--r--   0        0        0      797 2023-07-31 20:04:37.347287 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.347338 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2498 2023-07-31 20:04:37.347450 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0      995 2023-07-31 20:04:37.347620 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.347730 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0     5864 2023-07-31 20:04:37.347846 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/bank_pb2.py
--rw-r--r--   0        0        0     3705 2023-07-31 20:04:37.347946 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/bank_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.348020 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/bank_pb2_grpc.py
--rw-r--r--   0        0        0     4030 2023-07-31 20:04:37.348128 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2022 2023-07-31 20:04:37.348195 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.348254 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    16800 2023-07-31 20:04:37.348321 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     8496 2023-07-31 20:04:37.348398 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    21828 2023-07-31 20:04:37.348486 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     6614 2023-07-31 20:04:37.348582 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2992 2023-07-31 20:04:37.348706 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     8074 2023-07-31 20:04:37.348844 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     6904 2023-07-31 20:04:37.349072 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/abci/v1beta1/abci_pb2.py
--rw-r--r--   0        0        0     6040 2023-07-31 20:04:37.349151 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.349239 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.py
--rw-r--r--   0        0        0     1611 2023-07-31 20:04:37.349424 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/kv/v1beta1/kv_pb2.py
--rw-r--r--   0        0        0      895 2023-07-31 20:04:37.349506 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.349579 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.py
--rw-r--r--   0        0        0     1942 2023-07-31 20:04:37.349738 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2.py
--rw-r--r--   0        0        0      594 2023-07-31 20:04:37.349807 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     2762 2023-07-31 20:04:37.349893 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1581 2023-07-31 20:04:37.350042 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/query/v1beta1/pagination_pb2.py
--rw-r--r--   0        0        0     1063 2023-07-31 20:04:37.350121 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.350198 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.py
--rw-r--r--   0        0        0     3149 2023-07-31 20:04:37.350408 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py
--rw-r--r--   0        0        0     1325 2023-07-31 20:04:37.350571 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
--rw-r--r--   0        0        0     5144 2023-07-31 20:04:37.350680 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0    11054 2023-07-31 20:04:37.350799 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py
--rw-r--r--   0        0        0     8428 2023-07-31 20:04:37.350893 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
--rw-r--r--   0        0        0    13573 2023-07-31 20:04:37.350973 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0     4474 2023-07-31 20:04:37.351127 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
--rw-r--r--   0        0        0     3890 2023-07-31 20:04:37.351211 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.351274 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0     2232 2023-07-31 20:04:37.351424 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/store/v1beta1/commit_info_pb2.py
--rw-r--r--   0        0        0     1359 2023-07-31 20:04:37.351507 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.351574 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-07-31 20:04:37.351651 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/store/v1beta1/listening_pb2.py
--rw-r--r--   0        0        0     2675 2023-07-31 20:04:37.351724 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/store/v1beta1/listening_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.351797 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/store/v1beta1/listening_pb2_grpc.py
--rw-r--r--   0        0        0    11268 2023-07-31 20:04:37.351977 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     9082 2023-07-31 20:04:37.352080 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    14492 2023-07-31 20:04:37.352141 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4265 2023-07-31 20:04:37.352221 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/types_pb2.py
--rw-r--r--   0        0        0     3178 2023-07-31 20:04:37.352300 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.352360 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/types_pb2_grpc.py
--rw-r--r--   0        0        0     3182 2023-07-31 20:04:37.352464 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/v1beta1/coin_pb2.py
--rw-r--r--   0        0        0     1234 2023-07-31 20:04:37.352530 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/v1beta1/coin_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.352587 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
--rw-r--r--   0        0        0     1412 2023-07-31 20:04:37.352764 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/module/v1/module_pb2.py
--rw-r--r--   0        0        0      457 2023-07-31 20:04:37.353062 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.353154 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2222 2023-07-31 20:04:37.353298 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/v1beta1/capability_pb2.py
--rw-r--r--   0        0        0     1137 2023-07-31 20:04:37.353373 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/v1beta1/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.353436 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/v1beta1/capability_pb2_grpc.py
--rw-r--r--   0        0        0     2292 2023-07-31 20:04:37.353539 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1243 2023-07-31 20:04:37.353612 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.353677 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1401 2023-07-31 20:04:37.353866 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/module/v1/module_pb2.py
--rw-r--r--   0        0        0      458 2023-07-31 20:04:37.353935 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.353998 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2093 2023-07-31 20:04:37.354108 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/query_pb2.py
--rw-r--r--   0        0        0      719 2023-07-31 20:04:37.354185 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2626 2023-07-31 20:04:37.354241 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2479 2023-07-31 20:04:37.354303 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/tx_pb2.py
--rw-r--r--   0        0        0     1196 2023-07-31 20:04:37.354364 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     2734 2023-07-31 20:04:37.354432 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1440 2023-07-31 20:04:37.354598 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/module/v1/module_pb2.py
--rw-r--r--   0        0        0      602 2023-07-31 20:04:37.354708 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.354786 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1754 2023-07-31 20:04:37.354896 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      636 2023-07-31 20:04:37.354965 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.355028 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3990 2023-07-31 20:04:37.355104 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1539 2023-07-31 20:04:37.355166 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4533 2023-07-31 20:04:37.355229 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2315 2023-07-31 20:04:37.355382 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/ed25519/keys_pb2.py
--rw-r--r--   0        0        0      641 2023-07-31 20:04:37.355454 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/ed25519/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.355514 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/ed25519/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1753 2023-07-31 20:04:37.355672 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/hd/v1/hd_pb2.py
--rw-r--r--   0        0        0      902 2023-07-31 20:04:37.355746 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/hd/v1/hd_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.355806 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/hd/v1/hd_pb2_grpc.py
--rw-r--r--   0        0        0     2621 2023-07-31 20:04:37.355959 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/keyring/v1/record_pb2.py
--rw-r--r--   0        0        0     1911 2023-07-31 20:04:37.356038 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/keyring/v1/record_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.356102 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/keyring/v1/record_pb2_grpc.py
--rw-r--r--   0        0        0     2109 2023-07-31 20:04:37.356208 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/multisig/keys_pb2.py
--rw-r--r--   0        0        0      877 2023-07-31 20:04:37.356272 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/multisig/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.356326 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/multisig/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1797 2023-07-31 20:04:37.356426 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
--rw-r--r--   0        0        0      930 2023-07-31 20:04:37.356507 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.356570 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.py
--rw-r--r--   0        0        0     1944 2023-07-31 20:04:37.356677 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/secp256k1/keys_pb2.py
--rw-r--r--   0        0        0      641 2023-07-31 20:04:37.356740 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/secp256k1/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.356793 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/secp256k1/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1880 2023-07-31 20:04:37.356893 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/secp256r1/keys_pb2.py
--rw-r--r--   0        0        0      611 2023-07-31 20:04:37.356956 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/secp256r1/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.357009 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/secp256r1/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1475 2023-07-31 20:04:37.357155 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/module/v1/module_pb2.py
--rw-r--r--   0        0        0      602 2023-07-31 20:04:37.357210 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.357263 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0    10734 2023-07-31 20:04:37.357393 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/distribution_pb2.py
--rw-r--r--   0        0        0     5853 2023-07-31 20:04:37.357485 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.357553 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.py
--rw-r--r--   0        0        0    12723 2023-07-31 20:04:37.357613 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     6870 2023-07-31 20:04:37.357671 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.357735 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    19359 2023-07-31 20:04:37.357846 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     7387 2023-07-31 20:04:37.357941 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    20401 2023-07-31 20:04:37.358044 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0    10917 2023-07-31 20:04:37.358118 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     3979 2023-07-31 20:04:37.358176 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0    12766 2023-07-31 20:04:37.358237 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1359 2023-07-31 20:04:37.358386 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/module/v1/module_pb2.py
--rw-r--r--   0        0        0      329 2023-07-31 20:04:37.358444 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.358506 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2519 2023-07-31 20:04:37.358621 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/evidence_pb2.py
--rw-r--r--   0        0        0     1009 2023-07-31 20:04:37.358697 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.358759 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.py
--rw-r--r--   0        0        0     1360 2023-07-31 20:04:37.358822 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      666 2023-07-31 20:04:37.358885 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.358951 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3676 2023-07-31 20:04:37.359025 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1871 2023-07-31 20:04:37.359094 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4459 2023-07-31 20:04:37.359171 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3065 2023-07-31 20:04:37.359246 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1017 2023-07-31 20:04:37.359312 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2754 2023-07-31 20:04:37.359430 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1359 2023-07-31 20:04:37.359630 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/module/v1/module_pb2.py
--rw-r--r--   0        0        0      329 2023-07-31 20:04:37.359703 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.359776 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     6633 2023-07-31 20:04:37.359899 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py
--rw-r--r--   0        0        0     3059 2023-07-31 20:04:37.359981 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.360043 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.py
--rw-r--r--   0        0        0     1768 2023-07-31 20:04:37.360101 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      792 2023-07-31 20:04:37.360161 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.360220 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     5500 2023-07-31 20:04:37.360309 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     2919 2023-07-31 20:04:37.360378 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6420 2023-07-31 20:04:37.360444 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4250 2023-07-31 20:04:37.360529 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1385 2023-07-31 20:04:37.360590 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4601 2023-07-31 20:04:37.360668 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1351 2023-07-31 20:04:37.360861 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/genutil/module/v1/module_pb2.py
--rw-r--r--   0        0        0      329 2023-07-31 20:04:37.360925 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/genutil/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.360983 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/genutil/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1728 2023-07-31 20:04:37.361083 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/genutil/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      627 2023-07-31 20:04:37.361147 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.361208 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1413 2023-07-31 20:04:37.361396 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/module/v1/module_pb2.py
--rw-r--r--   0        0        0      594 2023-07-31 20:04:37.361467 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.361528 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2296 2023-07-31 20:04:37.361640 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1892 2023-07-31 20:04:37.361725 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.361784 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    10867 2023-07-31 20:04:37.361961 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/gov_pb2.py
--rw-r--r--   0        0        0     8798 2023-07-31 20:04:37.362079 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.362147 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/gov_pb2_grpc.py
--rw-r--r--   0        0        0     9988 2023-07-31 20:04:37.362264 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/query_pb2.py
--rw-r--r--   0        0        0     6461 2023-07-31 20:04:37.362345 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/query_pb2.pyi
--rw-r--r--   0        0        0    14263 2023-07-31 20:04:37.362644 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     9149 2023-07-31 20:04:37.362701 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/tx_pb2.py
--rw-r--r--   0        0        0     4680 2023-07-31 20:04:37.362790 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/tx_pb2.pyi
--rw-r--r--   0        0        0    11056 2023-07-31 20:04:37.362898 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3351 2023-07-31 20:04:37.363010 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1845 2023-07-31 20:04:37.363087 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.363147 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    15123 2023-07-31 20:04:37.363257 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/gov_pb2.py
--rw-r--r--   0        0        0     7002 2023-07-31 20:04:37.363331 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.363391 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/gov_pb2_grpc.py
--rw-r--r--   0        0        0    12489 2023-07-31 20:04:37.363452 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     6414 2023-07-31 20:04:37.363521 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    14598 2023-07-31 20:04:37.363582 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     8048 2023-07-31 20:04:37.363660 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     3221 2023-07-31 20:04:37.363738 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     7675 2023-07-31 20:04:37.363807 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2006 2023-07-31 20:04:37.364006 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/module/v1/module_pb2.py
--rw-r--r--   0        0        0      876 2023-07-31 20:04:37.364061 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.364121 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     3640 2023-07-31 20:04:37.364228 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/events_pb2.py
--rw-r--r--   0        0        0     2528 2023-07-31 20:04:37.364300 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.364354 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/events_pb2_grpc.py
--rw-r--r--   0        0        0     1762 2023-07-31 20:04:37.364424 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1930 2023-07-31 20:04:37.364486 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.364544 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    16091 2023-07-31 20:04:37.364595 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/query_pb2.py
--rw-r--r--   0        0        0    10177 2023-07-31 20:04:37.364652 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/query_pb2.pyi
--rw-r--r--   0        0        0    24311 2023-07-31 20:04:37.364766 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0    20329 2023-07-31 20:04:37.364905 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/tx_pb2.py
--rw-r--r--   0        0        0    10585 2023-07-31 20:04:37.364998 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/tx_pb2.pyi
--rw-r--r--   0        0        0    25421 2023-07-31 20:04:37.365068 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0    12022 2023-07-31 20:04:37.365168 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/types_pb2.py
--rw-r--r--   0        0        0    10059 2023-07-31 20:04:37.365249 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.365314 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/types_pb2_grpc.py
--rw-r--r--   0        0        0     1427 2023-07-31 20:04:37.365488 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/module/v1/module_pb2.py
--rw-r--r--   0        0        0      602 2023-07-31 20:04:37.365570 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.365639 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1992 2023-07-31 20:04:37.365742 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      756 2023-07-31 20:04:37.365826 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.365876 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3877 2023-07-31 20:04:37.365943 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/mint_pb2.py
--rw-r--r--   0        0        0     1527 2023-07-31 20:04:37.366009 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/mint_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.366071 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/mint_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-07-31 20:04:37.366127 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1462 2023-07-31 20:04:37.366186 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6210 2023-07-31 20:04:37.366248 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2878 2023-07-31 20:04:37.366307 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0      929 2023-07-31 20:04:37.366361 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2744 2023-07-31 20:04:37.366413 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1473 2023-07-31 20:04:37.366548 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/msg/v1/msg_pb2.py
--rw-r--r--   0        0        0      343 2023-07-31 20:04:37.366614 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/msg/v1/msg_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.366667 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/msg/v1/msg_pb2_grpc.py
--rw-r--r--   0        0        0     1328 2023-07-31 20:04:37.366811 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/module/v1/module_pb2.py
--rw-r--r--   0        0        0      329 2023-07-31 20:04:37.366865 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.366912 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1705 2023-07-31 20:04:37.367013 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/event_pb2.py
--rw-r--r--   0        0        0     1409 2023-07-31 20:04:37.367082 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.367141 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/event_pb2_grpc.py
--rw-r--r--   0        0        0     1610 2023-07-31 20:04:37.367196 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1204 2023-07-31 20:04:37.367254 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.367314 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1821 2023-07-31 20:04:37.367376 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/nft_pb2.py
--rw-r--r--   0        0        0     1648 2023-07-31 20:04:37.367432 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/nft_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.367493 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/nft_pb2_grpc.py
--rw-r--r--   0        0        0     6988 2023-07-31 20:04:37.367568 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     4396 2023-07-31 20:04:37.367628 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    12817 2023-07-31 20:04:37.367725 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2389 2023-07-31 20:04:37.367792 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0      871 2023-07-31 20:04:37.367851 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2511 2023-07-31 20:04:37.367907 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1350 2023-07-31 20:04:37.368070 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/module/v1alpha1/module_pb2.py
--rw-r--r--   0        0        0      329 2023-07-31 20:04:37.368124 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/module/v1alpha1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.368177 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/module/v1alpha1/module_pb2_grpc.py
--rw-r--r--   0        0        0     3962 2023-07-31 20:04:37.368316 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2.py
--rw-r--r--   0        0        0     4194 2023-07-31 20:04:37.368409 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2.pyi
--rw-r--r--   0        0        0     4388 2023-07-31 20:04:37.368465 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2410 2023-07-31 20:04:37.368561 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/v1/orm_pb2.py
--rw-r--r--   0        0        0     1952 2023-07-31 20:04:37.368638 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/v1/orm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.368693 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/v1/orm_pb2_grpc.py
--rw-r--r--   0        0        0     2210 2023-07-31 20:04:37.368787 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/v1alpha1/schema_pb2.py
--rw-r--r--   0        0        0     2023 2023-07-31 20:04:37.368857 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/v1alpha1/schema_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.368910 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/v1alpha1/schema_pb2_grpc.py
--rw-r--r--   0        0        0     1346 2023-07-31 20:04:37.369058 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/module/v1/module_pb2.py
--rw-r--r--   0        0        0      329 2023-07-31 20:04:37.369116 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.369173 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2587 2023-07-31 20:04:37.369275 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/params_pb2.py
--rw-r--r--   0        0        0     1339 2023-07-31 20:04:37.369341 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.369395 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/params_pb2_grpc.py
--rw-r--r--   0        0        0     3486 2023-07-31 20:04:37.369459 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1800 2023-07-31 20:04:37.369514 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4478 2023-07-31 20:04:37.369574 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1339 2023-07-31 20:04:37.369689 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/query/v1/query_pb2.py
--rw-r--r--   0        0        0      291 2023-07-31 20:04:37.369748 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/query/v1/query_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.369792 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/query/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2028 2023-07-31 20:04:37.369907 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2.py
--rw-r--r--   0        0        0      881 2023-07-31 20:04:37.369971 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2.pyi
--rw-r--r--   0        0        0     3070 2023-07-31 20:04:37.370030 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0     1396 2023-07-31 20:04:37.370182 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/module/v1/module_pb2.py
--rw-r--r--   0        0        0      458 2023-07-31 20:04:37.370242 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.370303 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4070 2023-07-31 20:04:37.370394 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2337 2023-07-31 20:04:37.370474 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.370537 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     5304 2023-07-31 20:04:37.370606 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     2345 2023-07-31 20:04:37.370664 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6284 2023-07-31 20:04:37.370716 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4472 2023-07-31 20:04:37.370783 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/slashing_pb2.py
--rw-r--r--   0        0        0     2340 2023-07-31 20:04:37.370853 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.370906 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.py
--rw-r--r--   0        0        0     3997 2023-07-31 20:04:37.370965 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1265 2023-07-31 20:04:37.371012 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4596 2023-07-31 20:04:37.371067 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1429 2023-07-31 20:04:37.371247 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/module/v1/module_pb2.py
--rw-r--r--   0        0        0      713 2023-07-31 20:04:37.371322 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.371380 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     3302 2023-07-31 20:04:37.371476 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     2201 2023-07-31 20:04:37.371543 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.371601 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0     4361 2023-07-31 20:04:37.371659 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2537 2023-07-31 20:04:37.371723 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.371780 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    24857 2023-07-31 20:04:37.371849 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    11419 2023-07-31 20:04:37.371960 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    27948 2023-07-31 20:04:37.372032 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0    25418 2023-07-31 20:04:37.372183 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/staking_pb2.py
--rw-r--r--   0        0        0    13772 2023-07-31 20:04:37.372300 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/staking_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.372358 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/staking_pb2_grpc.py
--rw-r--r--   0        0        0    15656 2023-07-31 20:04:37.372415 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     6326 2023-07-31 20:04:37.372484 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0    13680 2023-07-31 20:04:37.372547 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1431 2023-07-31 20:04:37.372706 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/config/v1/config_pb2.py
--rw-r--r--   0        0        0      612 2023-07-31 20:04:37.372767 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/config/v1/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.372827 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/config/v1/config_pb2_grpc.py
--rw-r--r--   0        0        0     3297 2023-07-31 20:04:37.372993 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/signing/v1beta1/signing_pb2.py
--rw-r--r--   0        0        0     3241 2023-07-31 20:04:37.373064 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.373119 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.py
--rw-r--r--   0        0        0    10727 2023-07-31 20:04:37.373229 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2.py
--rw-r--r--   0        0        0     7646 2023-07-31 20:04:37.373309 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2.pyi
--rw-r--r--   0        0        0    16593 2023-07-31 20:04:37.373402 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2_grpc.py
--rw-r--r--   0        0        0     6916 2023-07-31 20:04:37.373484 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     7626 2023-07-31 20:04:37.373554 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.373643 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1388 2023-07-31 20:04:37.373806 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/module/v1/module_pb2.py
--rw-r--r--   0        0        0      458 2023-07-31 20:04:37.373872 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.373937 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     5819 2023-07-31 20:04:37.374045 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     2589 2023-07-31 20:04:37.374110 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    10523 2023-07-31 20:04:37.374189 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3843 2023-07-31 20:04:37.374253 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1248 2023-07-31 20:04:37.374319 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4582 2023-07-31 20:04:37.374388 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     4397 2023-07-31 20:04:37.374465 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py
--rw-r--r--   0        0        0     2202 2023-07-31 20:04:37.374531 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.374591 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.py
--rw-r--r--   0        0        0     1361 2023-07-31 20:04:37.374784 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/module/v1/module_pb2.py
--rw-r--r--   0        0        0      329 2023-07-31 20:04:37.374851 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.374908 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     6899 2023-07-31 20:04:37.375018 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2935 2023-07-31 20:04:37.375111 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     6844 2023-07-31 20:04:37.375200 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     7340 2023-07-31 20:04:37.375288 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/vesting_pb2.py
--rw-r--r--   0        0        0     3611 2023-07-31 20:04:37.375361 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.375421 dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.py
--rw-r--r--   0        0        0     2861 2023-07-31 20:04:37.375588 dydxpy-0.3.0.post1/dydxpy/proto/cosmos_proto/cosmos_pb2.py
--rw-r--r--   0        0        0     2019 2023-07-31 20:04:37.375661 dydxpy-0.3.0.post1/dydxpy/proto/cosmos_proto/cosmos_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.375718 dydxpy-0.3.0.post1/dydxpy/proto/cosmos_proto/cosmos_pb2_grpc.py
--rw-r--r--   0        0        0     1484 2023-07-31 20:04:37.375864 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/asset_pb2.py
--rw-r--r--   0        0        0     1162 2023-07-31 20:04:37.375939 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/asset_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.375998 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/asset_pb2_grpc.py
--rw-r--r--   0        0        0     1615 2023-07-31 20:04:37.376060 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/genesis_pb2.py
--rw-r--r--   0        0        0      718 2023-07-31 20:04:37.376140 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.376206 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1143 2023-07-31 20:04:37.376272 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/query_pb2.py
--rw-r--r--   0        0        0      135 2023-07-31 20:04:37.376336 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/query_pb2.pyi
--rw-r--r--   0        0        0      988 2023-07-31 20:04:37.387724 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/query_pb2_grpc.py
--rw-r--r--   0        0        0     1128 2023-07-31 20:04:37.387833 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/tx_pb2.py
--rw-r--r--   0        0        0      135 2023-07-31 20:04:37.387899 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/tx_pb2.pyi
--rw-r--r--   0        0        0      978 2023-07-31 20:04:37.387977 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2582 2023-07-31 20:04:37.388079 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/blocktime_pb2.py
--rw-r--r--   0        0        0     1577 2023-07-31 20:04:37.388145 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/blocktime_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.388193 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/blocktime_pb2_grpc.py
--rw-r--r--   0        0        0     1642 2023-07-31 20:04:37.388269 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/genesis_pb2.py
--rw-r--r--   0        0        0      601 2023-07-31 20:04:37.388340 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.388389 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2023-07-31 20:04:37.388455 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/params_pb2.py
--rw-r--r--   0        0        0     1006 2023-07-31 20:04:37.388508 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.388554 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/params_pb2_grpc.py
--rw-r--r--   0        0        0     3789 2023-07-31 20:04:37.388611 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/query_pb2.py
--rw-r--r--   0        0        0     1596 2023-07-31 20:04:37.388664 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/query_pb2.pyi
--rw-r--r--   0        0        0     6328 2023-07-31 20:04:37.388723 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/query_pb2_grpc.py
--rw-r--r--   0        0        0     3583 2023-07-31 20:04:37.388791 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2.py
--rw-r--r--   0        0        0     1376 2023-07-31 20:04:37.388835 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2.pyi
--rw-r--r--   0        0        0     4510 2023-07-31 20:04:37.388885 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1992 2023-07-31 20:04:37.388965 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/bridge_event_pb2.py
--rw-r--r--   0        0        0      792 2023-07-31 20:04:37.389019 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/bridge_event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.389064 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/bridge_event_pb2_grpc.py
--rw-r--r--   0        0        0     2201 2023-07-31 20:04:37.389116 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/genesis_pb2.py
--rw-r--r--   0        0        0     1166 2023-07-31 20:04:37.389171 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.389220 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     2581 2023-07-31 20:04:37.389280 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/params_pb2.py
--rw-r--r--   0        0        0     1933 2023-07-31 20:04:37.389336 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.389382 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/params_pb2_grpc.py
--rw-r--r--   0        0        0     6101 2023-07-31 20:04:37.389500 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/query_pb2.py
--rw-r--r--   0        0        0     2128 2023-07-31 20:04:37.389571 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/query_pb2.pyi
--rw-r--r--   0        0        0    10067 2023-07-31 20:04:37.389631 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/query_pb2_grpc.py
--rw-r--r--   0        0        0     6802 2023-07-31 20:04:37.389702 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/tx_pb2.py
--rw-r--r--   0        0        0     2787 2023-07-31 20:04:37.389766 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/tx_pb2.pyi
--rw-r--r--   0        0        0     9716 2023-07-31 20:04:37.389833 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2723 2023-07-31 20:04:37.389930 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/block_rate_limit_config_pb2.py
--rw-r--r--   0        0        0     1879 2023-07-31 20:04:37.389987 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/block_rate_limit_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390038 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/block_rate_limit_config_pb2_grpc.py
--rw-r--r--   0        0        0     2475 2023-07-31 20:04:37.390106 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/clob_pair_pb2.py
--rw-r--r--   0        0        0     3016 2023-07-31 20:04:37.390160 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/clob_pair_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390205 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/clob_pair_pb2_grpc.py
--rw-r--r--   0        0        0     2533 2023-07-31 20:04:37.390265 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/genesis_pb2.py
--rw-r--r--   0        0        0     1460 2023-07-31 20:04:37.390314 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390361 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3102 2023-07-31 20:04:37.390415 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/liquidations_config_pb2.py
--rw-r--r--   0        0        0     2879 2023-07-31 20:04:37.390468 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/liquidations_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390516 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/liquidations_config_pb2_grpc.py
--rw-r--r--   0        0        0     2086 2023-07-31 20:04:37.390574 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/liquidations_pb2.py
--rw-r--r--   0        0        0     1487 2023-07-31 20:04:37.390633 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/liquidations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390700 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/liquidations_pb2_grpc.py
--rw-r--r--   0        0        0     5021 2023-07-31 20:04:37.390755 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/matches_pb2.py
--rw-r--r--   0        0        0     4051 2023-07-31 20:04:37.390817 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/matches_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390864 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/matches_pb2_grpc.py
--rw-r--r--   0        0        0     2564 2023-07-31 20:04:37.390923 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/operation_pb2.py
--rw-r--r--   0        0        0     2310 2023-07-31 20:04:37.390983 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/operation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.391034 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/operation_pb2_grpc.py
--rw-r--r--   0        0        0     6740 2023-07-31 20:04:37.391115 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/order_pb2.py
--rw-r--r--   0        0        0     6619 2023-07-31 20:04:37.391188 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/order_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.391236 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/order_pb2_grpc.py
--rw-r--r--   0        0        0     2334 2023-07-31 20:04:37.391285 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/order_removals_pb2.py
--rw-r--r--   0        0        0     2211 2023-07-31 20:04:37.391337 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/order_removals_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.391384 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/order_removals_pb2_grpc.py
--rw-r--r--   0        0        0     3537 2023-07-31 20:04:37.391450 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/process_proposer_matches_events_pb2.py
--rw-r--r--   0        0        0     2424 2023-07-31 20:04:37.391517 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/process_proposer_matches_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.391573 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/process_proposer_matches_events_pb2_grpc.py
--rw-r--r--   0        0        0     5534 2023-07-31 20:04:37.391636 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/query_pb2.py
--rw-r--r--   0        0        0     3032 2023-07-31 20:04:37.391705 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/query_pb2.pyi
--rw-r--r--   0        0        0     6155 2023-07-31 20:04:37.391752 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/query_pb2_grpc.py
--rw-r--r--   0        0        0     4069 2023-07-31 20:04:37.391813 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/tx_pb2.py
--rw-r--r--   0        0        0     2576 2023-07-31 20:04:37.391867 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/tx_pb2.pyi
--rw-r--r--   0        0        0     6039 2023-07-31 20:04:37.391910 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2193 2023-07-31 20:04:37.392035 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2.py
--rw-r--r--   0        0        0      901 2023-07-31 20:04:37.392114 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2.pyi
--rw-r--r--   0        0        0     2920 2023-07-31 20:04:37.392166 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2_grpc.py
--rw-r--r--   0        0        0     2301 2023-07-31 20:04:37.392242 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2.py
--rw-r--r--   0        0        0      914 2023-07-31 20:04:37.392316 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2.pyi
--rw-r--r--   0        0        0     3163 2023-07-31 20:04:37.392398 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2_grpc.py
--rw-r--r--   0        0        0     2826 2023-07-31 20:04:37.392482 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2.py
--rw-r--r--   0        0        0     1829 2023-07-31 20:04:37.392539 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2.pyi
--rw-r--r--   0        0        0     3021 2023-07-31 20:04:37.392601 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2_grpc.py
--rw-r--r--   0        0        0     1485 2023-07-31 20:04:37.392690 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/epoch_info_pb2.py
--rw-r--r--   0        0        0     1161 2023-07-31 20:04:37.392747 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/epoch_info_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.392795 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/epoch_info_pb2_grpc.py
--rw-r--r--   0        0        0     1653 2023-07-31 20:04:37.392854 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/genesis_pb2.py
--rw-r--r--   0        0        0      782 2023-07-31 20:04:37.392902 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.392943 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3767 2023-07-31 20:04:37.392995 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/query_pb2.py
--rw-r--r--   0        0        0     1836 2023-07-31 20:04:37.393035 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/query_pb2.pyi
--rw-r--r--   0        0        0     4346 2023-07-31 20:04:37.393082 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/query_pb2_grpc.py
--rw-r--r--   0        0        0     1637 2023-07-31 20:04:37.393156 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/genesis_pb2.py
--rw-r--r--   0        0        0      608 2023-07-31 20:04:37.393201 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.393243 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1714 2023-07-31 20:04:37.393289 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/params_pb2.py
--rw-r--r--   0        0        0     1648 2023-07-31 20:04:37.393333 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.393371 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/params_pb2_grpc.py
--rw-r--r--   0        0        0     3721 2023-07-31 20:04:37.393437 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/query_pb2.py
--rw-r--r--   0        0        0     1392 2023-07-31 20:04:37.393476 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/query_pb2.pyi
--rw-r--r--   0        0        0     4473 2023-07-31 20:04:37.393519 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/query_pb2_grpc.py
--rw-r--r--   0        0        0     2789 2023-07-31 20:04:37.393565 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2.py
--rw-r--r--   0        0        0      945 2023-07-31 20:04:37.393608 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2.pyi
--rw-r--r--   0        0        0     2757 2023-07-31 20:04:37.393682 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2_grpc.py
--rw-r--r--   0        0        0     8495 2023-07-31 20:04:37.393822 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/events/events_pb2.py
--rw-r--r--   0        0        0     9096 2023-07-31 20:04:37.393891 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.393947 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/events/events_pb2_grpc.py
--rw-r--r--   0        0        0     3301 2023-07-31 20:04:37.394149 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/indexer_manager/event_pb2.py
--rw-r--r--   0        0        0     3162 2023-07-31 20:04:37.394234 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/indexer_manager/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.394288 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/indexer_manager/event_pb2_grpc.py
--rw-r--r--   0        0        0     4395 2023-07-31 20:04:37.394389 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/off_chain_updates/off_chain_updates_pb2.py
--rw-r--r--   0        0        0     5833 2023-07-31 20:04:37.394458 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/off_chain_updates/off_chain_updates_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.394517 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/off_chain_updates/off_chain_updates_pb2_grpc.py
--rw-r--r--   0        0        0     3331 2023-07-31 20:04:37.394653 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/clob_pb2.py
--rw-r--r--   0        0        0     3287 2023-07-31 20:04:37.394733 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/clob_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.394789 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/clob_pb2_grpc.py
--rw-r--r--   0        0        0     3609 2023-07-31 20:04:37.394855 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/subaccount_pb2.py
--rw-r--r--   0        0        0     1588 2023-07-31 20:04:37.394916 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/subaccount_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.394969 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/subaccount_pb2_grpc.py
--rw-r--r--   0        0        0     1820 2023-07-31 20:04:37.395062 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/redis/redis_order_pb2.py
--rw-r--r--   0        0        0     1576 2023-07-31 20:04:37.395120 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/redis/redis_order_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.395166 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/redis/redis_order_pb2_grpc.py
--rw-r--r--   0        0        0     3062 2023-07-31 20:04:37.395251 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/socks/messages_pb2.py
--rw-r--r--   0        0        0     3907 2023-07-31 20:04:37.395322 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/socks/messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.395369 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/socks/messages_pb2_grpc.py
--rw-r--r--   0        0        0     2317 2023-07-31 20:04:37.395454 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/genesis_pb2.py
--rw-r--r--   0        0        0     1224 2023-07-31 20:04:37.395507 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.395556 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1332 2023-07-31 20:04:37.395612 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/params_pb2.py
--rw-r--r--   0        0        0      836 2023-07-31 20:04:37.395666 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.395721 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/params_pb2_grpc.py
--rw-r--r--   0        0        0     2971 2023-07-31 20:04:37.395786 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/perpetual_pb2.py
--rw-r--r--   0        0        0     3107 2023-07-31 20:04:37.395849 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/perpetual_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.395907 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/perpetual_pb2_grpc.py
--rw-r--r--   0        0        0     3798 2023-07-31 20:04:37.395979 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2.py
--rw-r--r--   0        0        0     1817 2023-07-31 20:04:37.396035 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2.pyi
--rw-r--r--   0        0        0     4424 2023-07-31 20:04:37.396086 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2_grpc.py
--rw-r--r--   0        0        0     2136 2023-07-31 20:04:37.396149 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2.py
--rw-r--r--   0        0        0     1098 2023-07-31 20:04:37.396222 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2.pyi
--rw-r--r--   0        0        0     2680 2023-07-31 20:04:37.396278 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2048 2023-07-31 20:04:37.396359 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/genesis_pb2.py
--rw-r--r--   0        0        0     1106 2023-07-31 20:04:37.396410 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.396458 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1433 2023-07-31 20:04:37.396511 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/market_param_pb2.py
--rw-r--r--   0        0        0      997 2023-07-31 20:04:37.396563 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/market_param_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.396613 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/market_param_pb2_grpc.py
--rw-r--r--   0        0        0     1286 2023-07-31 20:04:37.396669 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/market_price_pb2.py
--rw-r--r--   0        0        0      573 2023-07-31 20:04:37.396726 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/market_price_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.396782 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/market_price_pb2_grpc.py
--rw-r--r--   0        0        0     6147 2023-07-31 20:04:37.396831 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/query_pb2.py
--rw-r--r--   0        0        0     3245 2023-07-31 20:04:37.396889 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/query_pb2.pyi
--rw-r--r--   0        0        0     7886 2023-07-31 20:04:37.396949 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/query_pb2_grpc.py
--rw-r--r--   0        0        0     1931 2023-07-31 20:04:37.397010 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/tx_pb2.py
--rw-r--r--   0        0        0     1146 2023-07-31 20:04:37.397059 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/tx_pb2.pyi
--rw-r--r--   0        0        0     2682 2023-07-31 20:04:37.397106 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1621 2023-07-31 20:04:37.397188 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/genesis_pb2.py
--rw-r--r--   0        0        0      583 2023-07-31 20:04:37.397234 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.397283 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1379 2023-07-31 20:04:37.397333 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/params_pb2.py
--rw-r--r--   0        0        0      900 2023-07-31 20:04:37.397383 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.397433 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/params_pb2_grpc.py
--rw-r--r--   0        0        0     2358 2023-07-31 20:04:37.397484 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/query_pb2.py
--rw-r--r--   0        0        0      749 2023-07-31 20:04:37.397535 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/query_pb2.pyi
--rw-r--r--   0        0        0     2570 2023-07-31 20:04:37.397593 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/query_pb2_grpc.py
--rw-r--r--   0        0        0     1946 2023-07-31 20:04:37.397659 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/reward_share_pb2.py
--rw-r--r--   0        0        0      592 2023-07-31 20:04:37.397717 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/reward_share_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.397768 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/reward_share_pb2_grpc.py
--rw-r--r--   0        0        0     2582 2023-07-31 20:04:37.397821 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/tx_pb2.py
--rw-r--r--   0        0        0      896 2023-07-31 20:04:37.397871 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/tx_pb2.pyi
--rw-r--r--   0        0        0     2566 2023-07-31 20:04:37.397927 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1172 2023-07-31 20:04:37.398017 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/genesis_pb2.py
--rw-r--r--   0        0        0      277 2023-07-31 20:04:37.398086 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.398137 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1143 2023-07-31 20:04:37.398193 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/query_pb2.py
--rw-r--r--   0        0        0      135 2023-07-31 20:04:37.398246 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/query_pb2.pyi
--rw-r--r--   0        0        0      989 2023-07-31 20:04:37.398302 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/query_pb2_grpc.py
--rw-r--r--   0        0        0     3843 2023-07-31 20:04:37.398372 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/transfer_pb2.py
--rw-r--r--   0        0        0     2251 2023-07-31 20:04:37.398432 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/transfer_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.398493 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/transfer_pb2_grpc.py
--rw-r--r--   0        0        0     2421 2023-07-31 20:04:37.398557 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/tx_pb2.py
--rw-r--r--   0        0        0      898 2023-07-31 20:04:37.398613 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/tx_pb2.pyi
--rw-r--r--   0        0        0     6483 2023-07-31 20:04:37.398664 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1606 2023-07-31 20:04:37.398750 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/genesis_pb2.py
--rw-r--r--   0        0        0      581 2023-07-31 20:04:37.398800 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.398851 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1628 2023-07-31 20:04:37.398900 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/params_pb2.py
--rw-r--r--   0        0        0      620 2023-07-31 20:04:37.398948 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.398999 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/params_pb2_grpc.py
--rw-r--r--   0        0        0     4769 2023-07-31 20:04:37.399047 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/query_pb2.py
--rw-r--r--   0        0        0     1971 2023-07-31 20:04:37.399095 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/query_pb2.pyi
--rw-r--r--   0        0        0     7633 2023-07-31 20:04:37.399147 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/query_pb2_grpc.py
--rw-r--r--   0        0        0     2936 2023-07-31 20:04:37.399202 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/stats_pb2.py
--rw-r--r--   0        0        0     2726 2023-07-31 20:04:37.399264 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/stats_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.399321 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/stats_pb2_grpc.py
--rw-r--r--   0        0        0     2561 2023-07-31 20:04:37.399371 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/tx_pb2.py
--rw-r--r--   0        0        0      894 2023-07-31 20:04:37.399425 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/tx_pb2.pyi
--rw-r--r--   0        0        0     2544 2023-07-31 20:04:37.399482 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1717 2023-07-31 20:04:37.399579 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/asset_position_pb2.py
--rw-r--r--   0        0        0      647 2023-07-31 20:04:37.399642 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/asset_position_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.399697 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/asset_position_pb2_grpc.py
--rw-r--r--   0        0        0     1688 2023-07-31 20:04:37.399746 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/genesis_pb2.py
--rw-r--r--   0        0        0      773 2023-07-31 20:04:37.399797 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.399849 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     2074 2023-07-31 20:04:37.399906 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/perpetual_position_pb2.py
--rw-r--r--   0        0        0      703 2023-07-31 20:04:37.399964 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/perpetual_position_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.400010 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/perpetual_position_pb2_grpc.py
--rw-r--r--   0        0        0     4253 2023-07-31 20:04:37.400065 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2.py
--rw-r--r--   0        0        0     2000 2023-07-31 20:04:37.400113 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2.pyi
--rw-r--r--   0        0        0     4466 2023-07-31 20:04:37.400168 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2_grpc.py
--rw-r--r--   0        0        0     2352 2023-07-31 20:04:37.400237 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/subaccount_pb2.py
--rw-r--r--   0        0        0     1716 2023-07-31 20:04:37.400306 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/subaccount_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.400354 dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/subaccount_pb2_grpc.py
--rw-r--r--   0        0        0    14535 2023-07-31 20:04:37.400473 dydxpy-0.3.0.post1/dydxpy/proto/gogoproto/gogo_pb2.py
--rw-r--r--   0        0        0     6847 2023-07-31 20:04:37.400570 dydxpy-0.3.0.post1/dydxpy/proto/gogoproto/gogo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.400620 dydxpy-0.3.0.post1/dydxpy/proto/gogoproto/gogo_pb2_grpc.py
--rw-r--r--   0        0        0     1599 2023-07-31 20:04:37.400748 dydxpy-0.3.0.post1/dydxpy/proto/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      310 2023-07-31 20:04:37.400953 dydxpy-0.3.0.post1/dydxpy/proto/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.401020 dydxpy-0.3.0.post1/dydxpy/proto/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2216 2023-07-31 20:04:37.401095 dydxpy-0.3.0.post1/dydxpy/proto/google/api/http_pb2.py
--rw-r--r--   0        0        0     2272 2023-07-31 20:04:37.401159 dydxpy-0.3.0.post1/dydxpy/proto/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.401208 dydxpy-0.3.0.post1/dydxpy/proto/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0    25923 2023-07-31 20:04:37.401411 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/abci/types_pb2.py
--rw-r--r--   0        0        0    29255 2023-07-31 20:04:37.401584 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/abci/types_pb2.pyi
--rw-r--r--   0        0        0    27809 2023-07-31 20:04:37.401697 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/abci/types_pb2_grpc.py
--rw-r--r--   0        0        0     1506 2023-07-31 20:04:37.401812 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/crypto/keys_pb2.py
--rw-r--r--   0        0        0      555 2023-07-31 20:04:37.401912 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/crypto/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.401973 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/crypto/keys_pb2_grpc.py
--rw-r--r--   0        0        0     2342 2023-07-31 20:04:37.402040 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/crypto/proof_pb2.py
--rw-r--r--   0        0        0     2162 2023-07-31 20:04:37.402095 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/crypto/proof_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.402150 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/crypto/proof_pb2_grpc.py
--rw-r--r--   0        0        0     1260 2023-07-31 20:04:37.402274 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/libs/bits/types_pb2.py
--rw-r--r--   0        0        0      613 2023-07-31 20:04:37.402327 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/libs/bits/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.402383 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/libs/bits/types_pb2_grpc.py
--rw-r--r--   0        0        0     3595 2023-07-31 20:04:37.402496 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/p2p/types_pb2.py
--rw-r--r--   0        0        0     2374 2023-07-31 20:04:37.402625 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/p2p/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.402684 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/p2p/types_pb2_grpc.py
--rw-r--r--   0        0        0     2208 2023-07-31 20:04:37.402781 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/block_pb2.py
--rw-r--r--   0        0        0     1087 2023-07-31 20:04:37.402840 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/block_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.402889 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/block_pb2_grpc.py
--rw-r--r--   0        0        0     3628 2023-07-31 20:04:37.402949 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/evidence_pb2.py
--rw-r--r--   0        0        0     3204 2023-07-31 20:04:37.403038 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/evidence_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.403087 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/evidence_pb2_grpc.py
--rw-r--r--   0        0        0     3307 2023-07-31 20:04:37.403145 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/params_pb2.py
--rw-r--r--   0        0        0     2719 2023-07-31 20:04:37.403202 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.403252 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/params_pb2_grpc.py
--rw-r--r--   0        0        0    11359 2023-07-31 20:04:37.403333 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/types_pb2.py
--rw-r--r--   0        0        0     9772 2023-07-31 20:04:37.403420 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.403473 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/types_pb2_grpc.py
--rw-r--r--   0        0        0     2314 2023-07-31 20:04:37.403534 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/validator_pb2.py
--rw-r--r--   0        0        0     1962 2023-07-31 20:04:37.403592 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/validator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.403640 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/validator_pb2_grpc.py
--rw-r--r--   0        0        0     1612 2023-07-31 20:04:37.403731 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/version/types_pb2.py
--rw-r--r--   0        0        0      806 2023-07-31 20:04:37.403788 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/version/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-31 20:04:37.403835 dydxpy-0.3.0.post1/dydxpy/proto/tendermint/version/types_pb2_grpc.py
--rw-r--r--   0        0        0      536 2023-07-31 20:13:28.590430 dydxpy-0.3.0.post1/pyproject.toml
--rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 dydxpy-0.3.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1405 2023-07-17 13:45:23.246073 dydxpy-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1912 2023-07-31 20:27:16.516149 dydxpy-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 20:38:48.782587 dydxpy-0.3.1/dydxpy/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-31 20:03:17.669681 dydxpy-0.3.1/dydxpy/proto/__init__.py
+-rw-r--r--   0        0        0     1977 2023-07-31 20:04:37.339547 dydxpy-0.3.1/dydxpy/proto/amino/amino_pb2.py
+-rw-r--r--   0        0        0      601 2023-07-31 20:04:37.339691 dydxpy-0.3.1/dydxpy/proto/amino/amino_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.340662 dydxpy-0.3.1/dydxpy/proto/amino/amino_pb2_grpc.py
+-rw-r--r--   0        0        0     1964 2023-07-31 20:04:37.341030 dydxpy-0.3.1/dydxpy/proto/cosmos/app/runtime/v1alpha1/module_pb2.py
+-rw-r--r--   0        0        0     1860 2023-07-31 20:04:37.341134 dydxpy-0.3.1/dydxpy/proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.341213 dydxpy-0.3.1/dydxpy/proto/cosmos/app/runtime/v1alpha1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1798 2023-07-31 20:04:37.341326 dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/config_pb2.py
+-rw-r--r--   0        0        0     1769 2023-07-31 20:04:37.341404 dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.341606 dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/config_pb2_grpc.py
+-rw-r--r--   0        0        0     1961 2023-07-31 20:04:37.341744 dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/module_pb2.py
+-rw-r--r--   0        0        0     1597 2023-07-31 20:04:37.341849 dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.341926 dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1613 2023-07-31 20:04:37.342092 dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2.py
+-rw-r--r--   0        0        0      645 2023-07-31 20:04:37.342465 dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2.pyi
+-rw-r--r--   0        0        0     2603 2023-07-31 20:04:37.342624 dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1763 2023-07-31 20:04:37.342845 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1368 2023-07-31 20:04:37.342924 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.342995 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4477 2023-07-31 20:04:37.343140 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/auth_pb2.py
+-rw-r--r--   0        0        0     2825 2023-07-31 20:04:37.343232 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.343308 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/auth_pb2_grpc.py
+-rw-r--r--   0        0        0     1902 2023-07-31 20:04:37.343387 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      946 2023-07-31 20:04:37.343478 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.343544 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    12687 2023-07-31 20:04:37.343641 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     5358 2023-07-31 20:04:37.343731 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    19125 2023-07-31 20:04:37.344000 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2878 2023-07-31 20:04:37.344268 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0      929 2023-07-31 20:04:37.344491 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2743 2023-07-31 20:04:37.344626 dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1338 2023-07-31 20:04:37.344836 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      329 2023-07-31 20:04:37.345023 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.345131 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4042 2023-07-31 20:04:37.345297 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     2077 2023-07-31 20:04:37.345384 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.345456 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0     2375 2023-07-31 20:04:37.345540 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/event_pb2.py
+-rw-r--r--   0        0        0     1078 2023-07-31 20:04:37.345606 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.345667 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     1747 2023-07-31 20:04:37.345739 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      815 2023-07-31 20:04:37.345820 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.345878 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     5552 2023-07-31 20:04:37.346012 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     3422 2023-07-31 20:04:37.346120 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6331 2023-07-31 20:04:37.346219 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     5201 2023-07-31 20:04:37.346331 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2267 2023-07-31 20:04:37.346413 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6246 2023-07-31 20:04:37.346559 dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3978 2023-07-31 20:04:37.346713 dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/options_pb2.py
+-rw-r--r--   0        0        0     4987 2023-07-31 20:04:37.346798 dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/options_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.346864 dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/options_pb2_grpc.py
+-rw-r--r--   0        0        0     2467 2023-07-31 20:04:37.346958 dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/query_pb2.py
+-rw-r--r--   0        0        0     1197 2023-07-31 20:04:37.347015 dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2886 2023-07-31 20:04:37.347073 dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1426 2023-07-31 20:04:37.347223 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      797 2023-07-31 20:04:37.347287 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.347338 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2498 2023-07-31 20:04:37.347450 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0      995 2023-07-31 20:04:37.347620 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.347730 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0     5864 2023-07-31 20:04:37.347846 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/bank_pb2.py
+-rw-r--r--   0        0        0     3705 2023-07-31 20:04:37.347946 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/bank_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.348020 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/bank_pb2_grpc.py
+-rw-r--r--   0        0        0     4030 2023-07-31 20:04:37.348128 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2022 2023-07-31 20:04:37.348195 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.348254 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    16800 2023-07-31 20:04:37.348321 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     8496 2023-07-31 20:04:37.348398 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    21828 2023-07-31 20:04:37.348486 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     6614 2023-07-31 20:04:37.348582 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2992 2023-07-31 20:04:37.348706 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     8074 2023-07-31 20:04:37.348844 dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     6904 2023-07-31 20:04:37.349072 dydxpy-0.3.1/dydxpy/proto/cosmos/base/abci/v1beta1/abci_pb2.py
+-rw-r--r--   0        0        0     6040 2023-07-31 20:04:37.349151 dydxpy-0.3.1/dydxpy/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.349239 dydxpy-0.3.1/dydxpy/proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.py
+-rw-r--r--   0        0        0     1611 2023-07-31 20:04:37.349424 dydxpy-0.3.1/dydxpy/proto/cosmos/base/kv/v1beta1/kv_pb2.py
+-rw-r--r--   0        0        0      895 2023-07-31 20:04:37.349506 dydxpy-0.3.1/dydxpy/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.349579 dydxpy-0.3.1/dydxpy/proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.py
+-rw-r--r--   0        0        0     1942 2023-07-31 20:04:37.349738 dydxpy-0.3.1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0      594 2023-07-31 20:04:37.349807 dydxpy-0.3.1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     2762 2023-07-31 20:04:37.349893 dydxpy-0.3.1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1581 2023-07-31 20:04:37.350042 dydxpy-0.3.1/dydxpy/proto/cosmos/base/query/v1beta1/pagination_pb2.py
+-rw-r--r--   0        0        0     1063 2023-07-31 20:04:37.350121 dydxpy-0.3.1/dydxpy/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.350198 dydxpy-0.3.1/dydxpy/proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.py
+-rw-r--r--   0        0        0     3149 2023-07-31 20:04:37.350408 dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py
+-rw-r--r--   0        0        0     1325 2023-07-31 20:04:37.350571 dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
+-rw-r--r--   0        0        0     5144 2023-07-31 20:04:37.350680 dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0    11054 2023-07-31 20:04:37.350799 dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py
+-rw-r--r--   0        0        0     8428 2023-07-31 20:04:37.350893 dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
+-rw-r--r--   0        0        0    13573 2023-07-31 20:04:37.350973 dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0     4474 2023-07-31 20:04:37.351127 dydxpy-0.3.1/dydxpy/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
+-rw-r--r--   0        0        0     3890 2023-07-31 20:04:37.351211 dydxpy-0.3.1/dydxpy/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.351274 dydxpy-0.3.1/dydxpy/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0     2232 2023-07-31 20:04:37.351424 dydxpy-0.3.1/dydxpy/proto/cosmos/base/store/v1beta1/commit_info_pb2.py
+-rw-r--r--   0        0        0     1359 2023-07-31 20:04:37.351507 dydxpy-0.3.1/dydxpy/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.351574 dydxpy-0.3.1/dydxpy/proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-07-31 20:04:37.351651 dydxpy-0.3.1/dydxpy/proto/cosmos/base/store/v1beta1/listening_pb2.py
+-rw-r--r--   0        0        0     2675 2023-07-31 20:04:37.351724 dydxpy-0.3.1/dydxpy/proto/cosmos/base/store/v1beta1/listening_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.351797 dydxpy-0.3.1/dydxpy/proto/cosmos/base/store/v1beta1/listening_pb2_grpc.py
+-rw-r--r--   0        0        0    11268 2023-07-31 20:04:37.351977 dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     9082 2023-07-31 20:04:37.352080 dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    14492 2023-07-31 20:04:37.352141 dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4265 2023-07-31 20:04:37.352221 dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/types_pb2.py
+-rw-r--r--   0        0        0     3178 2023-07-31 20:04:37.352300 dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.352360 dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/types_pb2_grpc.py
+-rw-r--r--   0        0        0     3182 2023-07-31 20:04:37.352464 dydxpy-0.3.1/dydxpy/proto/cosmos/base/v1beta1/coin_pb2.py
+-rw-r--r--   0        0        0     1234 2023-07-31 20:04:37.352530 dydxpy-0.3.1/dydxpy/proto/cosmos/base/v1beta1/coin_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.352587 dydxpy-0.3.1/dydxpy/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
+-rw-r--r--   0        0        0     1412 2023-07-31 20:04:37.352764 dydxpy-0.3.1/dydxpy/proto/cosmos/capability/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      457 2023-07-31 20:04:37.353062 dydxpy-0.3.1/dydxpy/proto/cosmos/capability/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.353154 dydxpy-0.3.1/dydxpy/proto/cosmos/capability/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2222 2023-07-31 20:04:37.353298 dydxpy-0.3.1/dydxpy/proto/cosmos/capability/v1beta1/capability_pb2.py
+-rw-r--r--   0        0        0     1137 2023-07-31 20:04:37.353373 dydxpy-0.3.1/dydxpy/proto/cosmos/capability/v1beta1/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.353436 dydxpy-0.3.1/dydxpy/proto/cosmos/capability/v1beta1/capability_pb2_grpc.py
+-rw-r--r--   0        0        0     2292 2023-07-31 20:04:37.353539 dydxpy-0.3.1/dydxpy/proto/cosmos/capability/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1243 2023-07-31 20:04:37.353612 dydxpy-0.3.1/dydxpy/proto/cosmos/capability/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.353677 dydxpy-0.3.1/dydxpy/proto/cosmos/capability/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1401 2023-07-31 20:04:37.353866 dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      458 2023-07-31 20:04:37.353935 dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.353998 dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2093 2023-07-31 20:04:37.354108 dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/query_pb2.py
+-rw-r--r--   0        0        0      719 2023-07-31 20:04:37.354185 dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2626 2023-07-31 20:04:37.354241 dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2479 2023-07-31 20:04:37.354303 dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/tx_pb2.py
+-rw-r--r--   0        0        0     1196 2023-07-31 20:04:37.354364 dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2734 2023-07-31 20:04:37.354432 dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1440 2023-07-31 20:04:37.354598 dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      602 2023-07-31 20:04:37.354708 dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.354786 dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1754 2023-07-31 20:04:37.354896 dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      636 2023-07-31 20:04:37.354965 dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.355028 dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3990 2023-07-31 20:04:37.355104 dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1539 2023-07-31 20:04:37.355166 dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4533 2023-07-31 20:04:37.355229 dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2315 2023-07-31 20:04:37.355382 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/ed25519/keys_pb2.py
+-rw-r--r--   0        0        0      641 2023-07-31 20:04:37.355454 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/ed25519/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.355514 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/ed25519/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1753 2023-07-31 20:04:37.355672 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/hd/v1/hd_pb2.py
+-rw-r--r--   0        0        0      902 2023-07-31 20:04:37.355746 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/hd/v1/hd_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.355806 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/hd/v1/hd_pb2_grpc.py
+-rw-r--r--   0        0        0     2621 2023-07-31 20:04:37.355959 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/keyring/v1/record_pb2.py
+-rw-r--r--   0        0        0     1911 2023-07-31 20:04:37.356038 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/keyring/v1/record_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.356102 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/keyring/v1/record_pb2_grpc.py
+-rw-r--r--   0        0        0     2109 2023-07-31 20:04:37.356208 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/multisig/keys_pb2.py
+-rw-r--r--   0        0        0      877 2023-07-31 20:04:37.356272 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/multisig/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.356326 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/multisig/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1797 2023-07-31 20:04:37.356426 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
+-rw-r--r--   0        0        0      930 2023-07-31 20:04:37.356507 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.356570 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.py
+-rw-r--r--   0        0        0     1944 2023-07-31 20:04:37.356677 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/secp256k1/keys_pb2.py
+-rw-r--r--   0        0        0      641 2023-07-31 20:04:37.356740 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/secp256k1/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.356793 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/secp256k1/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1880 2023-07-31 20:04:37.356893 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/secp256r1/keys_pb2.py
+-rw-r--r--   0        0        0      611 2023-07-31 20:04:37.356956 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/secp256r1/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.357009 dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/secp256r1/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1475 2023-07-31 20:04:37.357155 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      602 2023-07-31 20:04:37.357210 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.357263 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0    10734 2023-07-31 20:04:37.357393 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/distribution_pb2.py
+-rw-r--r--   0        0        0     5853 2023-07-31 20:04:37.357485 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.357553 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.py
+-rw-r--r--   0        0        0    12723 2023-07-31 20:04:37.357613 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     6870 2023-07-31 20:04:37.357671 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.357735 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    19359 2023-07-31 20:04:37.357846 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     7387 2023-07-31 20:04:37.357941 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    20401 2023-07-31 20:04:37.358044 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    10917 2023-07-31 20:04:37.358118 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3979 2023-07-31 20:04:37.358176 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0    12766 2023-07-31 20:04:37.358237 dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1359 2023-07-31 20:04:37.358386 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      329 2023-07-31 20:04:37.358444 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.358506 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2519 2023-07-31 20:04:37.358621 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/evidence_pb2.py
+-rw-r--r--   0        0        0     1009 2023-07-31 20:04:37.358697 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.358759 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.py
+-rw-r--r--   0        0        0     1360 2023-07-31 20:04:37.358822 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      666 2023-07-31 20:04:37.358885 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.358951 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3676 2023-07-31 20:04:37.359025 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1871 2023-07-31 20:04:37.359094 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4459 2023-07-31 20:04:37.359171 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3065 2023-07-31 20:04:37.359246 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1017 2023-07-31 20:04:37.359312 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2754 2023-07-31 20:04:37.359430 dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1359 2023-07-31 20:04:37.359630 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      329 2023-07-31 20:04:37.359703 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.359776 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     6633 2023-07-31 20:04:37.359899 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py
+-rw-r--r--   0        0        0     3059 2023-07-31 20:04:37.359981 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.360043 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.py
+-rw-r--r--   0        0        0     1768 2023-07-31 20:04:37.360101 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      792 2023-07-31 20:04:37.360161 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.360220 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     5500 2023-07-31 20:04:37.360309 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     2919 2023-07-31 20:04:37.360378 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6420 2023-07-31 20:04:37.360444 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4250 2023-07-31 20:04:37.360529 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1385 2023-07-31 20:04:37.360590 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4601 2023-07-31 20:04:37.360668 dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1351 2023-07-31 20:04:37.360861 dydxpy-0.3.1/dydxpy/proto/cosmos/genutil/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      329 2023-07-31 20:04:37.360925 dydxpy-0.3.1/dydxpy/proto/cosmos/genutil/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.360983 dydxpy-0.3.1/dydxpy/proto/cosmos/genutil/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1728 2023-07-31 20:04:37.361083 dydxpy-0.3.1/dydxpy/proto/cosmos/genutil/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      627 2023-07-31 20:04:37.361147 dydxpy-0.3.1/dydxpy/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.361208 dydxpy-0.3.1/dydxpy/proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1413 2023-07-31 20:04:37.361396 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      594 2023-07-31 20:04:37.361467 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.361528 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2296 2023-07-31 20:04:37.361640 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1892 2023-07-31 20:04:37.361725 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.361784 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    10867 2023-07-31 20:04:37.361961 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/gov_pb2.py
+-rw-r--r--   0        0        0     8798 2023-07-31 20:04:37.362079 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.362147 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0     9988 2023-07-31 20:04:37.362264 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/query_pb2.py
+-rw-r--r--   0        0        0     6461 2023-07-31 20:04:37.362345 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    14263 2023-07-31 20:04:37.362644 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     9149 2023-07-31 20:04:37.362701 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/tx_pb2.py
+-rw-r--r--   0        0        0     4680 2023-07-31 20:04:37.362790 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0    11056 2023-07-31 20:04:37.362898 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3351 2023-07-31 20:04:37.363010 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1845 2023-07-31 20:04:37.363087 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.363147 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    15123 2023-07-31 20:04:37.363257 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/gov_pb2.py
+-rw-r--r--   0        0        0     7002 2023-07-31 20:04:37.363331 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.363391 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0    12489 2023-07-31 20:04:37.363452 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6414 2023-07-31 20:04:37.363521 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    14598 2023-07-31 20:04:37.363582 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     8048 2023-07-31 20:04:37.363660 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3221 2023-07-31 20:04:37.363738 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     7675 2023-07-31 20:04:37.363807 dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2006 2023-07-31 20:04:37.364006 dydxpy-0.3.1/dydxpy/proto/cosmos/group/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      876 2023-07-31 20:04:37.364061 dydxpy-0.3.1/dydxpy/proto/cosmos/group/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.364121 dydxpy-0.3.1/dydxpy/proto/cosmos/group/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     3640 2023-07-31 20:04:37.364228 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/events_pb2.py
+-rw-r--r--   0        0        0     2528 2023-07-31 20:04:37.364300 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.364354 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/events_pb2_grpc.py
+-rw-r--r--   0        0        0     1762 2023-07-31 20:04:37.364424 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1930 2023-07-31 20:04:37.364486 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.364544 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    16091 2023-07-31 20:04:37.364595 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/query_pb2.py
+-rw-r--r--   0        0        0    10177 2023-07-31 20:04:37.364652 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    24311 2023-07-31 20:04:37.364766 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    20329 2023-07-31 20:04:37.364905 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/tx_pb2.py
+-rw-r--r--   0        0        0    10585 2023-07-31 20:04:37.364998 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0    25421 2023-07-31 20:04:37.365068 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0    12022 2023-07-31 20:04:37.365168 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/types_pb2.py
+-rw-r--r--   0        0        0    10059 2023-07-31 20:04:37.365249 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.365314 dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/types_pb2_grpc.py
+-rw-r--r--   0        0        0     1427 2023-07-31 20:04:37.365488 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      602 2023-07-31 20:04:37.365570 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.365639 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1992 2023-07-31 20:04:37.365742 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      756 2023-07-31 20:04:37.365826 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.365876 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3877 2023-07-31 20:04:37.365943 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/mint_pb2.py
+-rw-r--r--   0        0        0     1527 2023-07-31 20:04:37.366009 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/mint_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.366071 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/mint_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-07-31 20:04:37.366127 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1462 2023-07-31 20:04:37.366186 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6210 2023-07-31 20:04:37.366248 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2878 2023-07-31 20:04:37.366307 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0      929 2023-07-31 20:04:37.366361 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2744 2023-07-31 20:04:37.366413 dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1473 2023-07-31 20:04:37.366548 dydxpy-0.3.1/dydxpy/proto/cosmos/msg/v1/msg_pb2.py
+-rw-r--r--   0        0        0      343 2023-07-31 20:04:37.366614 dydxpy-0.3.1/dydxpy/proto/cosmos/msg/v1/msg_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.366667 dydxpy-0.3.1/dydxpy/proto/cosmos/msg/v1/msg_pb2_grpc.py
+-rw-r--r--   0        0        0     1328 2023-07-31 20:04:37.366811 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      329 2023-07-31 20:04:37.366865 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.366912 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1705 2023-07-31 20:04:37.367013 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/event_pb2.py
+-rw-r--r--   0        0        0     1409 2023-07-31 20:04:37.367082 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.367141 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     1610 2023-07-31 20:04:37.367196 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1204 2023-07-31 20:04:37.367254 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.367314 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1821 2023-07-31 20:04:37.367376 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/nft_pb2.py
+-rw-r--r--   0        0        0     1648 2023-07-31 20:04:37.367432 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/nft_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.367493 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/nft_pb2_grpc.py
+-rw-r--r--   0        0        0     6988 2023-07-31 20:04:37.367568 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     4396 2023-07-31 20:04:37.367628 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    12817 2023-07-31 20:04:37.367725 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2389 2023-07-31 20:04:37.367792 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0      871 2023-07-31 20:04:37.367851 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2511 2023-07-31 20:04:37.367907 dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1350 2023-07-31 20:04:37.368070 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/module/v1alpha1/module_pb2.py
+-rw-r--r--   0        0        0      329 2023-07-31 20:04:37.368124 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/module/v1alpha1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.368177 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/module/v1alpha1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     3962 2023-07-31 20:04:37.368316 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2.py
+-rw-r--r--   0        0        0     4194 2023-07-31 20:04:37.368409 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2.pyi
+-rw-r--r--   0        0        0     4388 2023-07-31 20:04:37.368465 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2410 2023-07-31 20:04:37.368561 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/v1/orm_pb2.py
+-rw-r--r--   0        0        0     1952 2023-07-31 20:04:37.368638 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/v1/orm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.368693 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/v1/orm_pb2_grpc.py
+-rw-r--r--   0        0        0     2210 2023-07-31 20:04:37.368787 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/v1alpha1/schema_pb2.py
+-rw-r--r--   0        0        0     2023 2023-07-31 20:04:37.368857 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/v1alpha1/schema_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.368910 dydxpy-0.3.1/dydxpy/proto/cosmos/orm/v1alpha1/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     1346 2023-07-31 20:04:37.369058 dydxpy-0.3.1/dydxpy/proto/cosmos/params/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      329 2023-07-31 20:04:37.369116 dydxpy-0.3.1/dydxpy/proto/cosmos/params/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.369173 dydxpy-0.3.1/dydxpy/proto/cosmos/params/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2587 2023-07-31 20:04:37.369275 dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/params_pb2.py
+-rw-r--r--   0        0        0     1339 2023-07-31 20:04:37.369341 dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.369395 dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/params_pb2_grpc.py
+-rw-r--r--   0        0        0     3486 2023-07-31 20:04:37.369459 dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1800 2023-07-31 20:04:37.369514 dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4478 2023-07-31 20:04:37.369574 dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1339 2023-07-31 20:04:37.369689 dydxpy-0.3.1/dydxpy/proto/cosmos/query/v1/query_pb2.py
+-rw-r--r--   0        0        0      291 2023-07-31 20:04:37.369748 dydxpy-0.3.1/dydxpy/proto/cosmos/query/v1/query_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.369792 dydxpy-0.3.1/dydxpy/proto/cosmos/query/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2028 2023-07-31 20:04:37.369907 dydxpy-0.3.1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2.py
+-rw-r--r--   0        0        0      881 2023-07-31 20:04:37.369971 dydxpy-0.3.1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2.pyi
+-rw-r--r--   0        0        0     3070 2023-07-31 20:04:37.370030 dydxpy-0.3.1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0     1396 2023-07-31 20:04:37.370182 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      458 2023-07-31 20:04:37.370242 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.370303 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4070 2023-07-31 20:04:37.370394 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2337 2023-07-31 20:04:37.370474 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.370537 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     5304 2023-07-31 20:04:37.370606 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     2345 2023-07-31 20:04:37.370664 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6284 2023-07-31 20:04:37.370716 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4472 2023-07-31 20:04:37.370783 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/slashing_pb2.py
+-rw-r--r--   0        0        0     2340 2023-07-31 20:04:37.370853 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.370906 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.py
+-rw-r--r--   0        0        0     3997 2023-07-31 20:04:37.370965 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1265 2023-07-31 20:04:37.371012 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4596 2023-07-31 20:04:37.371067 dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1429 2023-07-31 20:04:37.371247 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      713 2023-07-31 20:04:37.371322 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.371380 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     3302 2023-07-31 20:04:37.371476 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     2201 2023-07-31 20:04:37.371543 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.371601 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0     4361 2023-07-31 20:04:37.371659 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2537 2023-07-31 20:04:37.371723 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.371780 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    24857 2023-07-31 20:04:37.371849 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    11419 2023-07-31 20:04:37.371960 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    27948 2023-07-31 20:04:37.372032 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    25418 2023-07-31 20:04:37.372183 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/staking_pb2.py
+-rw-r--r--   0        0        0    13772 2023-07-31 20:04:37.372300 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/staking_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.372358 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/staking_pb2_grpc.py
+-rw-r--r--   0        0        0    15656 2023-07-31 20:04:37.372415 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     6326 2023-07-31 20:04:37.372484 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0    13680 2023-07-31 20:04:37.372547 dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1431 2023-07-31 20:04:37.372706 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/config/v1/config_pb2.py
+-rw-r--r--   0        0        0      612 2023-07-31 20:04:37.372767 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/config/v1/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.372827 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/config/v1/config_pb2_grpc.py
+-rw-r--r--   0        0        0     3297 2023-07-31 20:04:37.372993 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/signing/v1beta1/signing_pb2.py
+-rw-r--r--   0        0        0     3241 2023-07-31 20:04:37.373064 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.373119 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.py
+-rw-r--r--   0        0        0    10727 2023-07-31 20:04:37.373229 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2.py
+-rw-r--r--   0        0        0     7646 2023-07-31 20:04:37.373309 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2.pyi
+-rw-r--r--   0        0        0    16593 2023-07-31 20:04:37.373402 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2_grpc.py
+-rw-r--r--   0        0        0     6916 2023-07-31 20:04:37.373484 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     7626 2023-07-31 20:04:37.373554 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.373643 dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1388 2023-07-31 20:04:37.373806 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      458 2023-07-31 20:04:37.373872 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.373937 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     5819 2023-07-31 20:04:37.374045 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     2589 2023-07-31 20:04:37.374110 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    10523 2023-07-31 20:04:37.374189 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3843 2023-07-31 20:04:37.374253 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1248 2023-07-31 20:04:37.374319 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4582 2023-07-31 20:04:37.374388 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     4397 2023-07-31 20:04:37.374465 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py
+-rw-r--r--   0        0        0     2202 2023-07-31 20:04:37.374531 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.374591 dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.py
+-rw-r--r--   0        0        0     1361 2023-07-31 20:04:37.374784 dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      329 2023-07-31 20:04:37.374851 dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.374908 dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     6899 2023-07-31 20:04:37.375018 dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2935 2023-07-31 20:04:37.375111 dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6844 2023-07-31 20:04:37.375200 dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     7340 2023-07-31 20:04:37.375288 dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/vesting_pb2.py
+-rw-r--r--   0        0        0     3611 2023-07-31 20:04:37.375361 dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.375421 dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.py
+-rw-r--r--   0        0        0     2861 2023-07-31 20:04:37.375588 dydxpy-0.3.1/dydxpy/proto/cosmos_proto/cosmos_pb2.py
+-rw-r--r--   0        0        0     2019 2023-07-31 20:04:37.375661 dydxpy-0.3.1/dydxpy/proto/cosmos_proto/cosmos_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.375718 dydxpy-0.3.1/dydxpy/proto/cosmos_proto/cosmos_pb2_grpc.py
+-rw-r--r--   0        0        0     1484 2023-07-31 20:04:37.375864 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/asset_pb2.py
+-rw-r--r--   0        0        0     1162 2023-07-31 20:04:37.375939 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/asset_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.375998 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/asset_pb2_grpc.py
+-rw-r--r--   0        0        0     1615 2023-07-31 20:04:37.376060 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/genesis_pb2.py
+-rw-r--r--   0        0        0      718 2023-07-31 20:04:37.376140 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.376206 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1143 2023-07-31 20:04:37.376272 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/query_pb2.py
+-rw-r--r--   0        0        0      135 2023-07-31 20:04:37.376336 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/query_pb2.pyi
+-rw-r--r--   0        0        0      988 2023-07-31 20:04:37.387724 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1128 2023-07-31 20:04:37.387833 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/tx_pb2.py
+-rw-r--r--   0        0        0      135 2023-07-31 20:04:37.387899 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/tx_pb2.pyi
+-rw-r--r--   0        0        0      978 2023-07-31 20:04:37.387977 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2582 2023-07-31 20:04:37.388079 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/blocktime_pb2.py
+-rw-r--r--   0        0        0     1577 2023-07-31 20:04:37.388145 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/blocktime_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.388193 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/blocktime_pb2_grpc.py
+-rw-r--r--   0        0        0     1642 2023-07-31 20:04:37.388269 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/genesis_pb2.py
+-rw-r--r--   0        0        0      601 2023-07-31 20:04:37.388340 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.388389 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2023-07-31 20:04:37.388455 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/params_pb2.py
+-rw-r--r--   0        0        0     1006 2023-07-31 20:04:37.388508 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.388554 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/params_pb2_grpc.py
+-rw-r--r--   0        0        0     3789 2023-07-31 20:04:37.388611 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/query_pb2.py
+-rw-r--r--   0        0        0     1596 2023-07-31 20:04:37.388664 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/query_pb2.pyi
+-rw-r--r--   0        0        0     6328 2023-07-31 20:04:37.388723 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3583 2023-07-31 20:04:37.388791 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2.py
+-rw-r--r--   0        0        0     1376 2023-07-31 20:04:37.388835 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2.pyi
+-rw-r--r--   0        0        0     4510 2023-07-31 20:04:37.388885 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1992 2023-07-31 20:04:37.388965 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/bridge_event_pb2.py
+-rw-r--r--   0        0        0      792 2023-07-31 20:04:37.389019 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/bridge_event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.389064 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/bridge_event_pb2_grpc.py
+-rw-r--r--   0        0        0     2201 2023-07-31 20:04:37.389116 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/genesis_pb2.py
+-rw-r--r--   0        0        0     1166 2023-07-31 20:04:37.389171 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.389220 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     2581 2023-07-31 20:04:37.389280 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/params_pb2.py
+-rw-r--r--   0        0        0     1933 2023-07-31 20:04:37.389336 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.389382 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/params_pb2_grpc.py
+-rw-r--r--   0        0        0     6101 2023-07-31 20:04:37.389500 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/query_pb2.py
+-rw-r--r--   0        0        0     2128 2023-07-31 20:04:37.389571 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/query_pb2.pyi
+-rw-r--r--   0        0        0    10067 2023-07-31 20:04:37.389631 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/query_pb2_grpc.py
+-rw-r--r--   0        0        0     6802 2023-07-31 20:04:37.389702 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/tx_pb2.py
+-rw-r--r--   0        0        0     2787 2023-07-31 20:04:37.389766 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/tx_pb2.pyi
+-rw-r--r--   0        0        0     9716 2023-07-31 20:04:37.389833 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2723 2023-07-31 20:04:37.389930 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/block_rate_limit_config_pb2.py
+-rw-r--r--   0        0        0     1879 2023-07-31 20:04:37.389987 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/block_rate_limit_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390038 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/block_rate_limit_config_pb2_grpc.py
+-rw-r--r--   0        0        0     2475 2023-07-31 20:04:37.390106 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/clob_pair_pb2.py
+-rw-r--r--   0        0        0     3016 2023-07-31 20:04:37.390160 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/clob_pair_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390205 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/clob_pair_pb2_grpc.py
+-rw-r--r--   0        0        0     2533 2023-07-31 20:04:37.390265 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/genesis_pb2.py
+-rw-r--r--   0        0        0     1460 2023-07-31 20:04:37.390314 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390361 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3102 2023-07-31 20:04:37.390415 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/liquidations_config_pb2.py
+-rw-r--r--   0        0        0     2879 2023-07-31 20:04:37.390468 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/liquidations_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390516 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/liquidations_config_pb2_grpc.py
+-rw-r--r--   0        0        0     2086 2023-07-31 20:04:37.390574 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/liquidations_pb2.py
+-rw-r--r--   0        0        0     1487 2023-07-31 20:04:37.390633 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/liquidations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390700 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/liquidations_pb2_grpc.py
+-rw-r--r--   0        0        0     5021 2023-07-31 20:04:37.390755 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/matches_pb2.py
+-rw-r--r--   0        0        0     4051 2023-07-31 20:04:37.390817 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/matches_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.390864 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/matches_pb2_grpc.py
+-rw-r--r--   0        0        0     2564 2023-07-31 20:04:37.390923 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/operation_pb2.py
+-rw-r--r--   0        0        0     2310 2023-07-31 20:04:37.390983 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/operation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.391034 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/operation_pb2_grpc.py
+-rw-r--r--   0        0        0     6740 2023-07-31 20:04:37.391115 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/order_pb2.py
+-rw-r--r--   0        0        0     6619 2023-07-31 20:04:37.391188 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/order_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.391236 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/order_pb2_grpc.py
+-rw-r--r--   0        0        0     2334 2023-07-31 20:04:37.391285 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/order_removals_pb2.py
+-rw-r--r--   0        0        0     2211 2023-07-31 20:04:37.391337 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/order_removals_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.391384 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/order_removals_pb2_grpc.py
+-rw-r--r--   0        0        0     3537 2023-07-31 20:04:37.391450 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/process_proposer_matches_events_pb2.py
+-rw-r--r--   0        0        0     2424 2023-07-31 20:04:37.391517 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/process_proposer_matches_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.391573 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/process_proposer_matches_events_pb2_grpc.py
+-rw-r--r--   0        0        0     5534 2023-07-31 20:04:37.391636 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/query_pb2.py
+-rw-r--r--   0        0        0     3032 2023-07-31 20:04:37.391705 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/query_pb2.pyi
+-rw-r--r--   0        0        0     6155 2023-07-31 20:04:37.391752 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4069 2023-07-31 20:04:37.391813 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/tx_pb2.py
+-rw-r--r--   0        0        0     2576 2023-07-31 20:04:37.391867 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/tx_pb2.pyi
+-rw-r--r--   0        0        0     6039 2023-07-31 20:04:37.391910 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2193 2023-07-31 20:04:37.392035 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2.py
+-rw-r--r--   0        0        0      901 2023-07-31 20:04:37.392114 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2.pyi
+-rw-r--r--   0        0        0     2920 2023-07-31 20:04:37.392166 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2_grpc.py
+-rw-r--r--   0        0        0     2301 2023-07-31 20:04:37.392242 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2.py
+-rw-r--r--   0        0        0      914 2023-07-31 20:04:37.392316 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2.pyi
+-rw-r--r--   0        0        0     3163 2023-07-31 20:04:37.392398 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2_grpc.py
+-rw-r--r--   0        0        0     2826 2023-07-31 20:04:37.392482 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2.py
+-rw-r--r--   0        0        0     1829 2023-07-31 20:04:37.392539 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2.pyi
+-rw-r--r--   0        0        0     3021 2023-07-31 20:04:37.392601 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2_grpc.py
+-rw-r--r--   0        0        0     1485 2023-07-31 20:04:37.392690 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/epoch_info_pb2.py
+-rw-r--r--   0        0        0     1161 2023-07-31 20:04:37.392747 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/epoch_info_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.392795 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/epoch_info_pb2_grpc.py
+-rw-r--r--   0        0        0     1653 2023-07-31 20:04:37.392854 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/genesis_pb2.py
+-rw-r--r--   0        0        0      782 2023-07-31 20:04:37.392902 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.392943 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3767 2023-07-31 20:04:37.392995 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/query_pb2.py
+-rw-r--r--   0        0        0     1836 2023-07-31 20:04:37.393035 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/query_pb2.pyi
+-rw-r--r--   0        0        0     4346 2023-07-31 20:04:37.393082 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1637 2023-07-31 20:04:37.393156 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/genesis_pb2.py
+-rw-r--r--   0        0        0      608 2023-07-31 20:04:37.393201 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.393243 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1714 2023-07-31 20:04:37.393289 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/params_pb2.py
+-rw-r--r--   0        0        0     1648 2023-07-31 20:04:37.393333 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.393371 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/params_pb2_grpc.py
+-rw-r--r--   0        0        0     3721 2023-07-31 20:04:37.393437 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/query_pb2.py
+-rw-r--r--   0        0        0     1392 2023-07-31 20:04:37.393476 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/query_pb2.pyi
+-rw-r--r--   0        0        0     4473 2023-07-31 20:04:37.393519 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2789 2023-07-31 20:04:37.393565 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2.py
+-rw-r--r--   0        0        0      945 2023-07-31 20:04:37.393608 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2.pyi
+-rw-r--r--   0        0        0     2757 2023-07-31 20:04:37.393682 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     8495 2023-07-31 20:04:37.393822 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/events/events_pb2.py
+-rw-r--r--   0        0        0     9096 2023-07-31 20:04:37.393891 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.393947 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0     3301 2023-07-31 20:04:37.394149 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/indexer_manager/event_pb2.py
+-rw-r--r--   0        0        0     3162 2023-07-31 20:04:37.394234 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/indexer_manager/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.394288 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/indexer_manager/event_pb2_grpc.py
+-rw-r--r--   0        0        0     4395 2023-07-31 20:04:37.394389 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/off_chain_updates/off_chain_updates_pb2.py
+-rw-r--r--   0        0        0     5833 2023-07-31 20:04:37.394458 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/off_chain_updates/off_chain_updates_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.394517 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/off_chain_updates/off_chain_updates_pb2_grpc.py
+-rw-r--r--   0        0        0     3331 2023-07-31 20:04:37.394653 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/clob_pb2.py
+-rw-r--r--   0        0        0     3287 2023-07-31 20:04:37.394733 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/clob_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.394789 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/clob_pb2_grpc.py
+-rw-r--r--   0        0        0     3609 2023-07-31 20:04:37.394855 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/subaccount_pb2.py
+-rw-r--r--   0        0        0     1588 2023-07-31 20:04:37.394916 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/subaccount_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.394969 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/subaccount_pb2_grpc.py
+-rw-r--r--   0        0        0     1820 2023-07-31 20:04:37.395062 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/redis/redis_order_pb2.py
+-rw-r--r--   0        0        0     1576 2023-07-31 20:04:37.395120 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/redis/redis_order_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.395166 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/redis/redis_order_pb2_grpc.py
+-rw-r--r--   0        0        0     3062 2023-07-31 20:04:37.395251 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/socks/messages_pb2.py
+-rw-r--r--   0        0        0     3907 2023-07-31 20:04:37.395322 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/socks/messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.395369 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/socks/messages_pb2_grpc.py
+-rw-r--r--   0        0        0     2317 2023-07-31 20:04:37.395454 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/genesis_pb2.py
+-rw-r--r--   0        0        0     1224 2023-07-31 20:04:37.395507 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.395556 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1332 2023-07-31 20:04:37.395612 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/params_pb2.py
+-rw-r--r--   0        0        0      836 2023-07-31 20:04:37.395666 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.395721 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/params_pb2_grpc.py
+-rw-r--r--   0        0        0     2971 2023-07-31 20:04:37.395786 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/perpetual_pb2.py
+-rw-r--r--   0        0        0     3107 2023-07-31 20:04:37.395849 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/perpetual_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.395907 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/perpetual_pb2_grpc.py
+-rw-r--r--   0        0        0     3798 2023-07-31 20:04:37.395979 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2.py
+-rw-r--r--   0        0        0     1817 2023-07-31 20:04:37.396035 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2.pyi
+-rw-r--r--   0        0        0     4424 2023-07-31 20:04:37.396086 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2136 2023-07-31 20:04:37.396149 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2.py
+-rw-r--r--   0        0        0     1098 2023-07-31 20:04:37.396222 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2.pyi
+-rw-r--r--   0        0        0     2680 2023-07-31 20:04:37.396278 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2048 2023-07-31 20:04:37.396359 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/genesis_pb2.py
+-rw-r--r--   0        0        0     1106 2023-07-31 20:04:37.396410 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.396458 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1433 2023-07-31 20:04:37.396511 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/market_param_pb2.py
+-rw-r--r--   0        0        0      997 2023-07-31 20:04:37.396563 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/market_param_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.396613 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/market_param_pb2_grpc.py
+-rw-r--r--   0        0        0     1286 2023-07-31 20:04:37.396669 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/market_price_pb2.py
+-rw-r--r--   0        0        0      573 2023-07-31 20:04:37.396726 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/market_price_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.396782 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/market_price_pb2_grpc.py
+-rw-r--r--   0        0        0     6147 2023-07-31 20:04:37.396831 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/query_pb2.py
+-rw-r--r--   0        0        0     3245 2023-07-31 20:04:37.396889 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/query_pb2.pyi
+-rw-r--r--   0        0        0     7886 2023-07-31 20:04:37.396949 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1931 2023-07-31 20:04:37.397010 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/tx_pb2.py
+-rw-r--r--   0        0        0     1146 2023-07-31 20:04:37.397059 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/tx_pb2.pyi
+-rw-r--r--   0        0        0     2682 2023-07-31 20:04:37.397106 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1621 2023-07-31 20:04:37.397188 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/genesis_pb2.py
+-rw-r--r--   0        0        0      583 2023-07-31 20:04:37.397234 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.397283 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1379 2023-07-31 20:04:37.397333 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/params_pb2.py
+-rw-r--r--   0        0        0      900 2023-07-31 20:04:37.397383 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.397433 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/params_pb2_grpc.py
+-rw-r--r--   0        0        0     2358 2023-07-31 20:04:37.397484 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/query_pb2.py
+-rw-r--r--   0        0        0      749 2023-07-31 20:04:37.397535 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/query_pb2.pyi
+-rw-r--r--   0        0        0     2570 2023-07-31 20:04:37.397593 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1946 2023-07-31 20:04:37.397659 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/reward_share_pb2.py
+-rw-r--r--   0        0        0      592 2023-07-31 20:04:37.397717 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/reward_share_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.397768 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/reward_share_pb2_grpc.py
+-rw-r--r--   0        0        0     2582 2023-07-31 20:04:37.397821 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/tx_pb2.py
+-rw-r--r--   0        0        0      896 2023-07-31 20:04:37.397871 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/tx_pb2.pyi
+-rw-r--r--   0        0        0     2566 2023-07-31 20:04:37.397927 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1172 2023-07-31 20:04:37.398017 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/genesis_pb2.py
+-rw-r--r--   0        0        0      277 2023-07-31 20:04:37.398086 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.398137 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1143 2023-07-31 20:04:37.398193 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/query_pb2.py
+-rw-r--r--   0        0        0      135 2023-07-31 20:04:37.398246 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/query_pb2.pyi
+-rw-r--r--   0        0        0      989 2023-07-31 20:04:37.398302 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3843 2023-07-31 20:04:37.398372 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/transfer_pb2.py
+-rw-r--r--   0        0        0     2251 2023-07-31 20:04:37.398432 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/transfer_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.398493 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/transfer_pb2_grpc.py
+-rw-r--r--   0        0        0     2421 2023-07-31 20:04:37.398557 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/tx_pb2.py
+-rw-r--r--   0        0        0      898 2023-07-31 20:04:37.398613 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/tx_pb2.pyi
+-rw-r--r--   0        0        0     6483 2023-07-31 20:04:37.398664 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1606 2023-07-31 20:04:37.398750 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/genesis_pb2.py
+-rw-r--r--   0        0        0      581 2023-07-31 20:04:37.398800 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.398851 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1628 2023-07-31 20:04:37.398900 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/params_pb2.py
+-rw-r--r--   0        0        0      620 2023-07-31 20:04:37.398948 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.398999 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/params_pb2_grpc.py
+-rw-r--r--   0        0        0     4769 2023-07-31 20:04:37.399047 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/query_pb2.py
+-rw-r--r--   0        0        0     1971 2023-07-31 20:04:37.399095 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/query_pb2.pyi
+-rw-r--r--   0        0        0     7633 2023-07-31 20:04:37.399147 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2936 2023-07-31 20:04:37.399202 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/stats_pb2.py
+-rw-r--r--   0        0        0     2726 2023-07-31 20:04:37.399264 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/stats_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.399321 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/stats_pb2_grpc.py
+-rw-r--r--   0        0        0     2561 2023-07-31 20:04:37.399371 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/tx_pb2.py
+-rw-r--r--   0        0        0      894 2023-07-31 20:04:37.399425 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/tx_pb2.pyi
+-rw-r--r--   0        0        0     2544 2023-07-31 20:04:37.399482 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1717 2023-07-31 20:04:37.399579 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/asset_position_pb2.py
+-rw-r--r--   0        0        0      647 2023-07-31 20:04:37.399642 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/asset_position_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.399697 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/asset_position_pb2_grpc.py
+-rw-r--r--   0        0        0     1688 2023-07-31 20:04:37.399746 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/genesis_pb2.py
+-rw-r--r--   0        0        0      773 2023-07-31 20:04:37.399797 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.399849 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     2074 2023-07-31 20:04:37.399906 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/perpetual_position_pb2.py
+-rw-r--r--   0        0        0      703 2023-07-31 20:04:37.399964 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/perpetual_position_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.400010 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/perpetual_position_pb2_grpc.py
+-rw-r--r--   0        0        0     4253 2023-07-31 20:04:37.400065 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2.py
+-rw-r--r--   0        0        0     2000 2023-07-31 20:04:37.400113 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2.pyi
+-rw-r--r--   0        0        0     4466 2023-07-31 20:04:37.400168 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2352 2023-07-31 20:04:37.400237 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/subaccount_pb2.py
+-rw-r--r--   0        0        0     1716 2023-07-31 20:04:37.400306 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/subaccount_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.400354 dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/subaccount_pb2_grpc.py
+-rw-r--r--   0        0        0    14535 2023-07-31 20:04:37.400473 dydxpy-0.3.1/dydxpy/proto/gogoproto/gogo_pb2.py
+-rw-r--r--   0        0        0     6847 2023-07-31 20:04:37.400570 dydxpy-0.3.1/dydxpy/proto/gogoproto/gogo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.400620 dydxpy-0.3.1/dydxpy/proto/gogoproto/gogo_pb2_grpc.py
+-rw-r--r--   0        0        0     1599 2023-07-31 20:04:37.400748 dydxpy-0.3.1/dydxpy/proto/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      310 2023-07-31 20:04:37.400953 dydxpy-0.3.1/dydxpy/proto/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.401020 dydxpy-0.3.1/dydxpy/proto/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2216 2023-07-31 20:04:37.401095 dydxpy-0.3.1/dydxpy/proto/google/api/http_pb2.py
+-rw-r--r--   0        0        0     2272 2023-07-31 20:04:37.401159 dydxpy-0.3.1/dydxpy/proto/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.401208 dydxpy-0.3.1/dydxpy/proto/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0    25923 2023-07-31 20:04:37.401411 dydxpy-0.3.1/dydxpy/proto/tendermint/abci/types_pb2.py
+-rw-r--r--   0        0        0    29255 2023-07-31 20:04:37.401584 dydxpy-0.3.1/dydxpy/proto/tendermint/abci/types_pb2.pyi
+-rw-r--r--   0        0        0    27809 2023-07-31 20:04:37.401697 dydxpy-0.3.1/dydxpy/proto/tendermint/abci/types_pb2_grpc.py
+-rw-r--r--   0        0        0     1506 2023-07-31 20:04:37.401812 dydxpy-0.3.1/dydxpy/proto/tendermint/crypto/keys_pb2.py
+-rw-r--r--   0        0        0      555 2023-07-31 20:04:37.401912 dydxpy-0.3.1/dydxpy/proto/tendermint/crypto/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.401973 dydxpy-0.3.1/dydxpy/proto/tendermint/crypto/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     2342 2023-07-31 20:04:37.402040 dydxpy-0.3.1/dydxpy/proto/tendermint/crypto/proof_pb2.py
+-rw-r--r--   0        0        0     2162 2023-07-31 20:04:37.402095 dydxpy-0.3.1/dydxpy/proto/tendermint/crypto/proof_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.402150 dydxpy-0.3.1/dydxpy/proto/tendermint/crypto/proof_pb2_grpc.py
+-rw-r--r--   0        0        0     1260 2023-07-31 20:04:37.402274 dydxpy-0.3.1/dydxpy/proto/tendermint/libs/bits/types_pb2.py
+-rw-r--r--   0        0        0      613 2023-07-31 20:04:37.402327 dydxpy-0.3.1/dydxpy/proto/tendermint/libs/bits/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.402383 dydxpy-0.3.1/dydxpy/proto/tendermint/libs/bits/types_pb2_grpc.py
+-rw-r--r--   0        0        0     3595 2023-07-31 20:04:37.402496 dydxpy-0.3.1/dydxpy/proto/tendermint/p2p/types_pb2.py
+-rw-r--r--   0        0        0     2374 2023-07-31 20:04:37.402625 dydxpy-0.3.1/dydxpy/proto/tendermint/p2p/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.402684 dydxpy-0.3.1/dydxpy/proto/tendermint/p2p/types_pb2_grpc.py
+-rw-r--r--   0        0        0     2208 2023-07-31 20:04:37.402781 dydxpy-0.3.1/dydxpy/proto/tendermint/types/block_pb2.py
+-rw-r--r--   0        0        0     1087 2023-07-31 20:04:37.402840 dydxpy-0.3.1/dydxpy/proto/tendermint/types/block_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.402889 dydxpy-0.3.1/dydxpy/proto/tendermint/types/block_pb2_grpc.py
+-rw-r--r--   0        0        0     3628 2023-07-31 20:04:37.402949 dydxpy-0.3.1/dydxpy/proto/tendermint/types/evidence_pb2.py
+-rw-r--r--   0        0        0     3204 2023-07-31 20:04:37.403038 dydxpy-0.3.1/dydxpy/proto/tendermint/types/evidence_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.403087 dydxpy-0.3.1/dydxpy/proto/tendermint/types/evidence_pb2_grpc.py
+-rw-r--r--   0        0        0     3307 2023-07-31 20:04:37.403145 dydxpy-0.3.1/dydxpy/proto/tendermint/types/params_pb2.py
+-rw-r--r--   0        0        0     2719 2023-07-31 20:04:37.403202 dydxpy-0.3.1/dydxpy/proto/tendermint/types/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.403252 dydxpy-0.3.1/dydxpy/proto/tendermint/types/params_pb2_grpc.py
+-rw-r--r--   0        0        0    11359 2023-07-31 20:04:37.403333 dydxpy-0.3.1/dydxpy/proto/tendermint/types/types_pb2.py
+-rw-r--r--   0        0        0     9772 2023-07-31 20:04:37.403420 dydxpy-0.3.1/dydxpy/proto/tendermint/types/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.403473 dydxpy-0.3.1/dydxpy/proto/tendermint/types/types_pb2_grpc.py
+-rw-r--r--   0        0        0     2314 2023-07-31 20:04:37.403534 dydxpy-0.3.1/dydxpy/proto/tendermint/types/validator_pb2.py
+-rw-r--r--   0        0        0     1962 2023-07-31 20:04:37.403592 dydxpy-0.3.1/dydxpy/proto/tendermint/types/validator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.403640 dydxpy-0.3.1/dydxpy/proto/tendermint/types/validator_pb2_grpc.py
+-rw-r--r--   0        0        0     1612 2023-07-31 20:04:37.403731 dydxpy-0.3.1/dydxpy/proto/tendermint/version/types_pb2.py
+-rw-r--r--   0        0        0      806 2023-07-31 20:04:37.403788 dydxpy-0.3.1/dydxpy/proto/tendermint/version/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-31 20:04:37.403835 dydxpy-0.3.1/dydxpy/proto/tendermint/version/types_pb2_grpc.py
+-rw-r--r--   0        0        0      530 2023-07-31 20:27:16.516343 dydxpy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2571 1970-01-01 00:00:00.000000 dydxpy-0.3.1/PKG-INFO
```

### Comparing `dydxpy-0.3.0.post1/LICENSE` & `dydxpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/README.md` & `dydxpy-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -87,8 +87,8 @@
   ```
 
 ## License
 
 Copyright © 2023 dYdX Trading Inc. (https://dydx.exchange/)
 
 Originally released dYdX Trading Inc. under: <br />
-Proprietary License © 2023 dYdX Trading Inc. <br />
+Proprietary License <br />
```

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/amino/amino_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/amino/amino_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/amino/amino_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/amino/amino_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/runtime/v1alpha1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/app/runtime/v1alpha1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/config_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/config_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/module_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/app/v1alpha1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/module/v1/module_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/auth_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/auth_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/auth/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/authz_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/authz_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/event_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/event_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/options_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/options_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/options_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/autocli/v1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/autocli/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/module/v1/module_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/authz_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/authz_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/bank_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/bank_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/bank_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/bank_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/abci/v1beta1/abci_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/abci/v1beta1/abci_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/kv/v1beta1/kv_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/kv/v1beta1/kv_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/node/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/query/v1beta1/pagination_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/query/v1beta1/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/store/v1beta1/commit_info_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/store/v1beta1/commit_info_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/store/v1beta1/listening_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/store/v1beta1/listening_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/store/v1beta1/listening_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/store/v1beta1/listening_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/types_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/v1beta1/coin_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/v1beta1/coin_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/base/v1beta1/coin_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/base/v1beta1/coin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/capability/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/v1beta1/capability_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/capability/v1beta1/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/v1beta1/capability_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/capability/v1beta1/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/capability/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/capability/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/capability/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/consensus/v1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/consensus/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/module/v1/module_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/ed25519/keys_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/ed25519/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/ed25519/keys_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/ed25519/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/hd/v1/hd_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/hd/v1/hd_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/hd/v1/hd_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/hd/v1/hd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/keyring/v1/record_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/keyring/v1/record_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/keyring/v1/record_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/keyring/v1/record_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/multisig/keys_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/multisig/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/multisig/keys_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/multisig/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/secp256k1/keys_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/secp256k1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/secp256k1/keys_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/secp256k1/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/secp256r1/keys_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/secp256r1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/crypto/secp256r1/keys_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/crypto/secp256r1/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/module/v1/module_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/distribution_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/evidence_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/genutil/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/genutil/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/genutil/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/genutil/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/module/v1/module_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/gov_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/gov_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/gov_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/gov_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/gov_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/gov_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/module/v1/module_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/events_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/events_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/events_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/types_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/group/v1/types_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/group/v1/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/module/v1/module_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/mint_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/mint_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/mint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/mint/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/msg/v1/msg_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/msg/v1/msg_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/event_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/event_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/nft_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/nft_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/nft_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/nft_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/nft/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/module/v1alpha1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/orm/module/v1alpha1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/v1/orm_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/orm/v1/orm_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/v1/orm_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/orm/v1/orm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/v1alpha1/schema_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/orm/v1alpha1/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/orm/v1alpha1/schema_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/orm/v1alpha1/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/params/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/params_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/params_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/params/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/params/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/query/v1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/query/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/reflection/v1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/slashing_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/slashing_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/module/v1/module_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/authz_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/authz_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/staking_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/staking_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/staking_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/staking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/config/v1/config_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/tx/config/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/config/v1/config_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/tx/config/v1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/signing/v1beta1/signing_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/tx/signing/v1beta1/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/tx/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/tx/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/module/v1/module_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/vesting_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/vesting_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos_proto/cosmos_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/cosmos_proto/cosmos_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/cosmos_proto/cosmos_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/cosmos_proto/cosmos_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/asset_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/asset_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/asset_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/asset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/assets/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/assets/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/blocktime_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/blocktime_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/blocktime_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/blocktime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/params_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/params_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/params_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/blocktime/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/bridge_event_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/bridge_event_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/bridge_event_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/bridge_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/params_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/params_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/params_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/bridge/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/bridge/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/block_rate_limit_config_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/block_rate_limit_config_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/block_rate_limit_config_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/block_rate_limit_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/clob_pair_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/clob_pair_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/clob_pair_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/clob_pair_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/liquidations_config_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/liquidations_config_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/liquidations_config_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/liquidations_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/liquidations_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/liquidations_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/liquidations_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/liquidations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/matches_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/matches_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/matches_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/matches_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/operation_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/operation_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/order_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/order_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/order_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/order_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/order_removals_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/order_removals_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/order_removals_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/order_removals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/process_proposer_matches_events_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/process_proposer_matches_events_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/process_proposer_matches_events_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/process_proposer_matches_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/clob/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/clob/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/bridge/bridge_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/liquidation/liquidation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/daemons/pricefeed/price_feed_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/epoch_info_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/epoch_info_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/epoch_info_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/epoch_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/epochs/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/epochs/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/params_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/params_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/params_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/feetiers/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/events/events_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/events/events_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/indexer_manager/event_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/indexer_manager/event_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/indexer_manager/event_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/indexer_manager/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/off_chain_updates/off_chain_updates_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/off_chain_updates/off_chain_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/off_chain_updates/off_chain_updates_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/off_chain_updates/off_chain_updates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/clob_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/clob_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/clob_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/clob_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/subaccount_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/subaccount_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/subaccount_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/protocol/v1/subaccount_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/redis/redis_order_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/redis/redis_order_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/redis/redis_order_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/redis/redis_order_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/socks/messages_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/socks/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/indexer/socks/messages_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/indexer/socks/messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/params_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/params_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/params_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/perpetual_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/perpetual_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/perpetual_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/perpetual_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/perpetuals/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/market_param_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/market_param_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/market_param_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/market_param_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/market_price_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/market_price_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/market_price_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/market_price_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/prices/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/prices/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/params_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/params_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/params_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/reward_share_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/reward_share_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/reward_share_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/reward_share_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/rewards/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/rewards/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/transfer_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/transfer_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/transfer_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/transfer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/sending/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/sending/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/params_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/params_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/params_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/stats_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/stats_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/stats_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/tx_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/tx_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/stats/tx_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/stats/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/asset_position_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/asset_position_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/asset_position_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/asset_position_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/genesis_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/genesis_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/perpetual_position_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/perpetual_position_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/perpetual_position_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/perpetual_position_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/subaccount_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/subaccount_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/dydxprotocol/subaccounts/subaccount_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/dydxprotocol/subaccounts/subaccount_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/gogoproto/gogo_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/gogoproto/gogo_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/google/api/annotations_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/google/api/http_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/google/api/http_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/abci/types_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/abci/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/abci/types_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/abci/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/abci/types_pb2_grpc.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/abci/types_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/crypto/keys_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/crypto/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/crypto/keys_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/crypto/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/crypto/proof_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/crypto/proof_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/crypto/proof_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/crypto/proof_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/libs/bits/types_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/libs/bits/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/libs/bits/types_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/libs/bits/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/p2p/types_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/p2p/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/p2p/types_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/p2p/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/block_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/types/block_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/block_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/types/block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/evidence_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/types/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/evidence_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/types/evidence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/params_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/types/params_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/params_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/types/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/types_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/types/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/types_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/types/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/validator_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/types/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/types/validator_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/types/validator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/version/types_pb2.py` & `dydxpy-0.3.1/dydxpy/proto/tendermint/version/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/dydxpy/proto/tendermint/version/types_pb2.pyi` & `dydxpy-0.3.1/dydxpy/proto/tendermint/version/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dydxpy-0.3.0.post1/pyproject.toml` & `dydxpy-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 
 [tool.setuptools]
 package-dir = {"" = "dydx"}
 
 [tool.poetry]
 name = "dydxpy"
-version = "0.3.0.post1"
+version = "0.3.1"
 description = "Proto types and clients for dYdX v4 protocol"
 authors = ["John Huang <contact@dydx.exchange>"]
 license = "MIT"
 readme = "README.md"
 include = ["dydxpy.egg-info/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `dydxpy-0.3.0.post1/PKG-INFO` & `dydxpy-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dydxpy
-Version: 0.3.0.post1
+Version: 0.3.1
 Summary: Proto types and clients for dYdX v4 protocol
 License: MIT
 Author: John Huang
 Author-email: contact@dydx.exchange
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -106,9 +106,9 @@
   ```
 
 ## License
 
 Copyright © 2023 dYdX Trading Inc. (https://dydx.exchange/)
 
 Originally released dYdX Trading Inc. under: <br />
-Proprietary License © 2023 dYdX Trading Inc. <br />
+Proprietary License <br />
```


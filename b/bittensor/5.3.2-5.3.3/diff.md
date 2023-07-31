# Comparing `tmp/bittensor-5.3.2.tar.gz` & `tmp/bittensor-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-5.3.2.tar", last modified: Wed Jul 26 22:40:30 2023, max compression
+gzip compressed data, was "bittensor-5.3.3.tar", last modified: Mon Jul 31 18:01:39 2023, max compression
```

## Comparing `bittensor-5.3.2.tar` & `bittensor-5.3.3.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.718769 bittensor-5.3.2/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1087 2023-07-13 19:44:57.000000 bittensor-5.3.2/LICENSE
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    23700 2023-07-26 22:40:30.717763 bittensor-5.3.2/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    22674 2023-07-26 22:21:01.000000 bittensor-5.3.2/README.md
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.662386 bittensor-5.3.2/bin/
--rwxr-xr-x   0 cameronfairchild   (501) staff       (20)     1297 2023-07-13 19:44:57.000000 bittensor-5.3.2/bin/btcli
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.662560 bittensor-5.3.2/bittensor/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    15269 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.663467 bittensor-5.3.2/bittensor/_axon/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    17340 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_axon/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.663841 bittensor-5.3.2/bittensor/_blacklist/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4771 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_blacklist/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.671583 bittensor-5.3.2/bittensor/_cli/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7239 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4389 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/cli_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.673737 bittensor-5.3.2/bittensor/_cli/commands/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      818 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    26908 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/delegates.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     8519 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/inspect.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4140 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/list.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     8316 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/metagraph.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6115 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/misc.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    19918 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/overview.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7705 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/register.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    18920 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/senate.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    11573 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/stake.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4519 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/transfer.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    11648 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/unstake.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     8338 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    18238 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_cli/commands/wallets.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.674448 bittensor-5.3.2/bittensor/_dataset/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    12379 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_dataset/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    28422 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_dataset/dataset_impl.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5476 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_dataset/dataset_mock.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3576 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_dataset/thread_queue.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.674701 bittensor-5.3.2/bittensor/_dendrite/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.2/bittensor/_dendrite/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    10414 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_dendrite/dendrite.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.675113 bittensor-5.3.2/bittensor/_dendrite/text_prompting/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.2/bittensor/_dendrite/text_prompting/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7933 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_dendrite/text_prompting/dendrite.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5059 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_dendrite/text_prompting/dendrite_pool.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.675357 bittensor-5.3.2/bittensor/_ipfs/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.2/bittensor/_ipfs/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     2981 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_ipfs/ipfs_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.675504 bittensor-5.3.2/bittensor/_logging/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    13552 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_logging/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.675650 bittensor-5.3.2/bittensor/_metagraph/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    14672 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_metagraph/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.676229 bittensor-5.3.2/bittensor/_neuron/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.2/bittensor/_neuron/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6781 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_neuron/base_huggingface_miner.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    10229 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_neuron/base_miner_neuron.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3279 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_neuron/base_prompting_miner.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.676365 bittensor-5.3.2/bittensor/_priority/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3472 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_priority/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.677017 bittensor-5.3.2/bittensor/_prometheus/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     8708 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_prometheus/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.677611 bittensor-5.3.2/bittensor/_proto/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.2/bittensor/_proto/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    35330 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_proto/bittensor_pb2.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4514 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_proto/bittensor_pb2_grpc.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.677928 bittensor-5.3.2/bittensor/_serializer/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6090 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_serializer/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    10579 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_serializer/serializer_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.678866 bittensor-5.3.2/bittensor/_subtensor/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    15625 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    26825 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/chain_data.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     2404 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/errors.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.682382 bittensor-5.3.2/bittensor/_subtensor/extrinsics/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1120 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    15299 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/delegation.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    30638 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/log_utilities.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6124 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/prometheus.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    13751 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/registration.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    11488 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/senate.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    10100 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/serving.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6198 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/set_weights.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    19392 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/staking.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6408 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/transfer.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    16524 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/extrinsics/unstaking.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    72174 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/subtensor_impl.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    52131 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/subtensor_mock.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1510 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_subtensor/types.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.682872 bittensor-5.3.2/bittensor/_synapse/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.2/bittensor/_synapse/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7252 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_synapse/synapse.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.683178 bittensor-5.3.2/bittensor/_synapse/text_prompting/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.2/bittensor/_synapse/text_prompting/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5281 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_synapse/text_prompting/synapse.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.683456 bittensor-5.3.2/bittensor/_threadpool/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5061 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_threadpool/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     8603 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_threadpool/priority_thread_pool_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.683612 bittensor-5.3.2/bittensor/_tokenizer/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     2458 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/_tokenizer/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.693901 bittensor-5.3.2/bittensor/utils/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6562 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3527 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/_register_cuda.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     8692 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/balance.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4432 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/codes.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      553 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/formatting.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7975 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/networking.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    39297 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/registration.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    34816 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/registratrion_old.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3302 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/stats.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      630 2023-07-13 19:44:57.000000 bittensor-5.3.2/bittensor/utils/test_utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    77419 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/tokenizer_utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     9940 2023-07-26 22:21:01.000000 bittensor-5.3.2/bittensor/utils/weight_utils.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.663329 bittensor-5.3.2/bittensor.egg-info/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    23700 2023-07-26 22:40:30.000000 bittensor-5.3.2/bittensor.egg-info/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4105 2023-07-26 22:40:30.000000 bittensor-5.3.2/bittensor.egg-info/SOURCES.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-07-26 22:40:30.000000 bittensor-5.3.2/bittensor.egg-info/dependency_links.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      922 2023-07-26 22:40:30.000000 bittensor-5.3.2/bittensor.egg-info/requires.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       16 2023-07-26 22:40:30.000000 bittensor-5.3.2/bittensor.egg-info/top_level.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-07-26 22:40:30.719449 bittensor-5.3.2/setup.cfg
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3425 2023-07-26 22:21:01.000000 bittensor-5.3.2/setup.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.694038 bittensor-5.3.2/tests/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1198 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.694304 bittensor-5.3.2/tests/helpers/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1275 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/helpers/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5423 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/helpers/helpers.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.707263 bittensor-5.3.2/tests/integration_tests/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:50:20.000000 bittensor-5.3.2/tests/integration_tests/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    80151 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/integration_tests/test_cli.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    42657 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/integration_tests/test_cli_no_network.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      969 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/integration_tests/test_ipfs.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3427 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/integration_tests/test_metagraph_integration.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1642 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/integration_tests/test_priority_thread_pool.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1440 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/integration_tests/test_prometheus.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    24522 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/integration_tests/test_subtensor_integration.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.707443 bittensor-5.3.2/tests/unit_tests/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:50:20.000000 bittensor-5.3.2/tests/unit_tests/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.716968 bittensor-5.3.2/tests/unit_tests/bittensor_tests/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:50:20.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    13893 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_axon.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    16019 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_balance.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4320 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_config.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1725 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_metagraph.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    13762 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_serialization.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6810 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_subtensor.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4947 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_synapse.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:40:30.717521 bittensor-5.3.2/tests/unit_tests/bittensor_tests/utils/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:50:20.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/utils/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5327 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/utils/test_network_utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    35864 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/utils/test_utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     2914 2023-07-26 22:21:01.000000 bittensor-5.3.2/tests/unit_tests/bittensor_tests/utils/test_weight_utils.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.025286 bittensor-5.3.3/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1087 2023-07-13 19:44:57.000000 bittensor-5.3.3/LICENSE
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    23700 2023-07-31 18:01:39.025082 bittensor-5.3.3/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    22674 2023-07-31 17:59:44.000000 bittensor-5.3.3/README.md
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:38.995669 bittensor-5.3.3/bin/
+-rwxr-xr-x   0 cameronfairchild   (501) staff       (20)     1297 2023-07-31 17:59:44.000000 bittensor-5.3.3/bin/btcli
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:38.995827 bittensor-5.3.3/bittensor/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    15269 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:38.997099 bittensor-5.3.3/bittensor/_axon/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    17340 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_axon/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:38.997547 bittensor-5.3.3/bittensor/_blacklist/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4771 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_blacklist/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:38.997938 bittensor-5.3.3/bittensor/_cli/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7239 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4389 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/cli_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.000229 bittensor-5.3.3/bittensor/_cli/commands/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      818 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    26908 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/delegates.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     8519 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/inspect.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4140 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/list.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     8316 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/metagraph.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6115 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/misc.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    19918 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/overview.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7705 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/register.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    18920 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/senate.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    11573 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/stake.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4519 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/transfer.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    11648 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/unstake.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     8338 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    18238 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_cli/commands/wallets.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.000862 bittensor-5.3.3/bittensor/_dataset/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    12379 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_dataset/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    28422 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_dataset/dataset_impl.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5476 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_dataset/dataset_mock.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3576 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_dataset/thread_queue.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.001202 bittensor-5.3.3/bittensor/_dendrite/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_dendrite/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    10414 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_dendrite/dendrite.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.001664 bittensor-5.3.3/bittensor/_dendrite/text_prompting/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_dendrite/text_prompting/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7933 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_dendrite/text_prompting/dendrite.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5059 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_dendrite/text_prompting/dendrite_pool.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.002331 bittensor-5.3.3/bittensor/_ipfs/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_ipfs/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     2981 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_ipfs/ipfs_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.002517 bittensor-5.3.3/bittensor/_logging/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    13552 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_logging/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.002682 bittensor-5.3.3/bittensor/_metagraph/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    14672 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_metagraph/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.003270 bittensor-5.3.3/bittensor/_neuron/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_neuron/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6781 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_neuron/base_huggingface_miner.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    10229 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_neuron/base_miner_neuron.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3279 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_neuron/base_prompting_miner.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.003407 bittensor-5.3.3/bittensor/_priority/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3472 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_priority/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.003580 bittensor-5.3.3/bittensor/_prometheus/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     8708 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_prometheus/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.004436 bittensor-5.3.3/bittensor/_proto/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_proto/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    35330 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_proto/bittensor_pb2.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4514 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_proto/bittensor_pb2_grpc.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.005266 bittensor-5.3.3/bittensor/_serializer/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6090 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_serializer/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    10579 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_serializer/serializer_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.006310 bittensor-5.3.3/bittensor/_subtensor/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    15625 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    26825 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/chain_data.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     2404 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/errors.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.008360 bittensor-5.3.3/bittensor/_subtensor/extrinsics/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1120 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    15299 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/delegation.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    30638 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/log_utilities.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6124 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/prometheus.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    13751 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/registration.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    11488 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/senate.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    10100 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/serving.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6198 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/set_weights.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    19392 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/staking.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6408 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/transfer.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    16524 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/extrinsics/unstaking.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    72174 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/subtensor_impl.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    52131 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/subtensor_mock.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1510 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_subtensor/types.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.008677 bittensor-5.3.3/bittensor/_synapse/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_synapse/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7252 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_synapse/synapse.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.009007 bittensor-5.3.3/bittensor/_synapse/text_prompting/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_synapse/text_prompting/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5281 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_synapse/text_prompting/synapse.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.009384 bittensor-5.3.3/bittensor/_threadpool/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5061 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_threadpool/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     8603 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_threadpool/priority_thread_pool_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.009581 bittensor-5.3.3/bittensor/_tokenizer/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     2458 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/_tokenizer/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.014612 bittensor-5.3.3/bittensor/utils/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6562 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/utils/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3527 2023-07-27 00:21:53.000000 bittensor-5.3.3/bittensor/utils/_register_cuda.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     8692 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/utils/balance.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4432 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/utils/codes.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      553 2023-07-27 00:21:53.000000 bittensor-5.3.3/bittensor/utils/formatting.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7975 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/utils/networking.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    39297 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/utils/registration.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    34816 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/utils/registratrion_old.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3302 2023-07-27 00:21:53.000000 bittensor-5.3.3/bittensor/utils/stats.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      630 2023-07-13 19:44:57.000000 bittensor-5.3.3/bittensor/utils/test_utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    77419 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/utils/tokenizer_utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     9940 2023-07-31 17:59:44.000000 bittensor-5.3.3/bittensor/utils/weight_utils.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:38.996743 bittensor-5.3.3/bittensor.egg-info/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    23700 2023-07-31 18:01:38.000000 bittensor-5.3.3/bittensor.egg-info/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4105 2023-07-31 18:01:38.000000 bittensor-5.3.3/bittensor.egg-info/SOURCES.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-07-31 18:01:38.000000 bittensor-5.3.3/bittensor.egg-info/dependency_links.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      905 2023-07-31 18:01:38.000000 bittensor-5.3.3/bittensor.egg-info/requires.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       16 2023-07-31 18:01:38.000000 bittensor-5.3.3/bittensor.egg-info/top_level.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-07-31 18:01:39.025338 bittensor-5.3.3/setup.cfg
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3425 2023-07-31 17:59:44.000000 bittensor-5.3.3/setup.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.014804 bittensor-5.3.3/tests/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1198 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.015733 bittensor-5.3.3/tests/helpers/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1275 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/helpers/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5423 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/helpers/helpers.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.017202 bittensor-5.3.3/tests/integration_tests/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-27 00:15:36.000000 bittensor-5.3.3/tests/integration_tests/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    80151 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/integration_tests/test_cli.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    42657 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/integration_tests/test_cli_no_network.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      969 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/integration_tests/test_ipfs.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3427 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/integration_tests/test_metagraph_integration.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1642 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/integration_tests/test_priority_thread_pool.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1440 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/integration_tests/test_prometheus.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    24522 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/integration_tests/test_subtensor_integration.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.017395 bittensor-5.3.3/tests/unit_tests/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-27 00:15:36.000000 bittensor-5.3.3/tests/unit_tests/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.024066 bittensor-5.3.3/tests/unit_tests/bittensor_tests/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    13893 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_axon.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    16019 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_balance.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4320 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_config.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1725 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_metagraph.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    13762 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_serialization.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6810 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_subtensor.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4947 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_synapse.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 18:01:39.024773 bittensor-5.3.3/tests/unit_tests/bittensor_tests/utils/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/utils/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5327 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/utils/test_network_utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    35864 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/utils/test_utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     2914 2023-07-31 17:59:44.000000 bittensor-5.3.3/tests/unit_tests/bittensor_tests/utils/test_weight_utils.py
```

### Comparing `bittensor-5.3.2/LICENSE` & `bittensor-5.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/PKG-INFO` & `bittensor-5.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 5.3.2
+Version: 5.3.3
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bittensor-5.3.2/README.md` & `bittensor-5.3.3/README.md`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bin/btcli` & `bittensor-5.3.3/bin/btcli`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/__init__.py` & `bittensor-5.3.3/bittensor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing import Optional, List, Mapping, Any, Tuple
 
 import nest_asyncio
 
 nest_asyncio.apply()
 
 # Bittensor code and protocol version.
-__version__ = "5.3.2"
+__version__ = "5.3.3"
 version_split = __version__.split(".")
 __version_as_int__ = (
     (100 * int(version_split[0]))
     + (10 * int(version_split[1]))
     + (1 * int(version_split[2]))
 )
 __new_signature_version__ = 360
```

### Comparing `bittensor-5.3.2/bittensor/_axon/__init__.py` & `bittensor-5.3.3/bittensor/_axon/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_blacklist/__init__.py` & `bittensor-5.3.3/bittensor/_blacklist/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/__init__.py` & `bittensor-5.3.3/bittensor/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/cli_impl.py` & `bittensor-5.3.3/bittensor/_cli/cli_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/__init__.py` & `bittensor-5.3.3/bittensor/_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/delegates.py` & `bittensor-5.3.3/bittensor/_cli/commands/delegates.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/inspect.py` & `bittensor-5.3.3/bittensor/_cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/list.py` & `bittensor-5.3.3/bittensor/_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/metagraph.py` & `bittensor-5.3.3/bittensor/_cli/commands/metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/misc.py` & `bittensor-5.3.3/bittensor/_cli/commands/misc.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/overview.py` & `bittensor-5.3.3/bittensor/_cli/commands/overview.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/register.py` & `bittensor-5.3.3/bittensor/_cli/commands/register.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/senate.py` & `bittensor-5.3.3/bittensor/_cli/commands/senate.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/stake.py` & `bittensor-5.3.3/bittensor/_cli/commands/stake.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/transfer.py` & `bittensor-5.3.3/bittensor/_cli/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/unstake.py` & `bittensor-5.3.3/bittensor/_cli/commands/unstake.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/utils.py` & `bittensor-5.3.3/bittensor/_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_cli/commands/wallets.py` & `bittensor-5.3.3/bittensor/_cli/commands/wallets.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_dataset/__init__.py` & `bittensor-5.3.3/bittensor/_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_dataset/dataset_impl.py` & `bittensor-5.3.3/bittensor/_dataset/dataset_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_dataset/dataset_mock.py` & `bittensor-5.3.3/bittensor/_dataset/dataset_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_dataset/thread_queue.py` & `bittensor-5.3.3/bittensor/_dataset/thread_queue.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_dendrite/dendrite.py` & `bittensor-5.3.3/bittensor/_dendrite/dendrite.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_dendrite/text_prompting/dendrite.py` & `bittensor-5.3.3/bittensor/_dendrite/text_prompting/dendrite.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_dendrite/text_prompting/dendrite_pool.py` & `bittensor-5.3.3/bittensor/_dendrite/text_prompting/dendrite_pool.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_ipfs/ipfs_impl.py` & `bittensor-5.3.3/bittensor/_ipfs/ipfs_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_logging/__init__.py` & `bittensor-5.3.3/bittensor/_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_metagraph/__init__.py` & `bittensor-5.3.3/bittensor/_metagraph/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_neuron/base_huggingface_miner.py` & `bittensor-5.3.3/bittensor/_neuron/base_huggingface_miner.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_neuron/base_miner_neuron.py` & `bittensor-5.3.3/bittensor/_neuron/base_miner_neuron.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_neuron/base_prompting_miner.py` & `bittensor-5.3.3/bittensor/_neuron/base_prompting_miner.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_priority/__init__.py` & `bittensor-5.3.3/bittensor/_priority/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_prometheus/__init__.py` & `bittensor-5.3.3/bittensor/_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_proto/bittensor_pb2.py` & `bittensor-5.3.3/bittensor/_proto/bittensor_pb2.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_proto/bittensor_pb2_grpc.py` & `bittensor-5.3.3/bittensor/_proto/bittensor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_serializer/__init__.py` & `bittensor-5.3.3/bittensor/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_serializer/serializer_impl.py` & `bittensor-5.3.3/bittensor/_serializer/serializer_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/__init__.py` & `bittensor-5.3.3/bittensor/_subtensor/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/chain_data.py` & `bittensor-5.3.3/bittensor/_subtensor/chain_data.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/errors.py` & `bittensor-5.3.3/bittensor/_subtensor/errors.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/__init__.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/delegation.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/delegation.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/log_utilities.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/log_utilities.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/prometheus.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/prometheus.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/registration.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/senate.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/senate.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/serving.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/serving.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/set_weights.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/set_weights.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/staking.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/staking.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/transfer.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/extrinsics/unstaking.py` & `bittensor-5.3.3/bittensor/_subtensor/extrinsics/unstaking.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/subtensor_impl.py` & `bittensor-5.3.3/bittensor/_subtensor/subtensor_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/subtensor_mock.py` & `bittensor-5.3.3/bittensor/_subtensor/subtensor_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_subtensor/types.py` & `bittensor-5.3.3/bittensor/_subtensor/types.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_synapse/synapse.py` & `bittensor-5.3.3/bittensor/_synapse/synapse.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_synapse/text_prompting/synapse.py` & `bittensor-5.3.3/bittensor/_synapse/text_prompting/synapse.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_threadpool/__init__.py` & `bittensor-5.3.3/bittensor/_threadpool/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_threadpool/priority_thread_pool_impl.py` & `bittensor-5.3.3/bittensor/_threadpool/priority_thread_pool_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/_tokenizer/__init__.py` & `bittensor-5.3.3/bittensor/_tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/__init__.py` & `bittensor-5.3.3/bittensor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/_register_cuda.py` & `bittensor-5.3.3/bittensor/utils/_register_cuda.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/balance.py` & `bittensor-5.3.3/bittensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/codes.py` & `bittensor-5.3.3/bittensor/utils/codes.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/formatting.py` & `bittensor-5.3.3/bittensor/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/networking.py` & `bittensor-5.3.3/bittensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/registration.py` & `bittensor-5.3.3/bittensor/utils/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/registratrion_old.py` & `bittensor-5.3.3/bittensor/utils/registratrion_old.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/stats.py` & `bittensor-5.3.3/bittensor/utils/stats.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/test_utils.py` & `bittensor-5.3.3/bittensor/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/tokenizer_utils.py` & `bittensor-5.3.3/bittensor/utils/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor/utils/weight_utils.py` & `bittensor-5.3.3/bittensor/utils/weight_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor.egg-info/PKG-INFO` & `bittensor-5.3.3/bittensor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 5.3.2
+Version: 5.3.3
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bittensor-5.3.2/bittensor.egg-info/SOURCES.txt` & `bittensor-5.3.3/bittensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/bittensor.egg-info/requires.txt` & `bittensor-5.3.3/bittensor.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 ansible_vault==2.1
 argparse==1.4.0
 base58==2.0.1
 backoff==2.1.0
-bittensor-config<1.0.0,>=0.0.1
-bittensor-wallet<1.0.0,>=0.0.5
+bittensor-config<1.0.0,>=0.0.0
+bittensor-wallet<1.0.0,==0.0.4
 cryptography==41.0.0
-datasets==2.12.0
 fuzzywuzzy==0.18.0
 grpcio==1.42.0
 grpcio-tools==1.42.0
 hypothesis==6.47.4
 idna<3,>=2.5
 jsonschema[format-nongpl]<=4.17.0,>=4.14.0
 langchain<=0.0.188,>=0.0.132
```

### Comparing `bittensor-5.3.2/setup.py` & `bittensor-5.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/__init__.py` & `bittensor-5.3.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/helpers/__init__.py` & `bittensor-5.3.3/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/helpers/helpers.py` & `bittensor-5.3.3/tests/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/integration_tests/test_cli.py` & `bittensor-5.3.3/tests/integration_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/integration_tests/test_cli_no_network.py` & `bittensor-5.3.3/tests/integration_tests/test_cli_no_network.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/integration_tests/test_ipfs.py` & `bittensor-5.3.3/tests/integration_tests/test_ipfs.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/integration_tests/test_metagraph_integration.py` & `bittensor-5.3.3/tests/integration_tests/test_metagraph_integration.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/integration_tests/test_priority_thread_pool.py` & `bittensor-5.3.3/tests/integration_tests/test_priority_thread_pool.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/integration_tests/test_prometheus.py` & `bittensor-5.3.3/tests/integration_tests/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/integration_tests/test_subtensor_integration.py` & `bittensor-5.3.3/tests/integration_tests/test_subtensor_integration.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_axon.py` & `bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_axon.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_balance.py` & `bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_config.py` & `bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_metagraph.py` & `bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_serialization.py` & `bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_subtensor.py` & `bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_subtensor.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/unit_tests/bittensor_tests/test_synapse.py` & `bittensor-5.3.3/tests/unit_tests/bittensor_tests/test_synapse.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/unit_tests/bittensor_tests/utils/test_network_utils.py` & `bittensor-5.3.3/tests/unit_tests/bittensor_tests/utils/test_network_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/unit_tests/bittensor_tests/utils/test_utils.py` & `bittensor-5.3.3/tests/unit_tests/bittensor_tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.2/tests/unit_tests/bittensor_tests/utils/test_weight_utils.py` & `bittensor-5.3.3/tests/unit_tests/bittensor_tests/utils/test_weight_utils.py`

 * *Files identical despite different names*


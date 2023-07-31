# Comparing `tmp/alpaca_eval-0.2.6.tar.gz` & `tmp/alpaca_eval-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.2.6.tar", last modified: Tue Jul 25 11:38:24 2023, max compression
+gzip compressed data, was "alpaca_eval-0.2.7.tar", last modified: Mon Jul 31 02:10:28 2023, max compression
```

## Comparing `alpaca_eval-0.2.6.tar` & `alpaca_eval-0.2.7.tar`

### file list

```diff
@@ -1,233 +1,234 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66618 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.367686 alpaca_eval-0.2.6/example/
--rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/example/outputs.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.339684 alpaca_eval-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.367686 alpaca_eval-0.2.6/src/alpaca_eval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 11:38:08.000000 alpaca_eval-0.2.6/src/alpaca_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval/annotators/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28020 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/annotators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/decoders/replicate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_2/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/test/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/test/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.375687 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.347684 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.363686 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/airoboros-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/airoboros-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baichuan-13b-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baize-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baize-v2-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/chatglm2-6b/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/claude-2/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/claude-2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/cohere/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/cohere/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/cohere-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.379687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/minotaur-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.383687 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-v2-w-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat8192-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/opencoderplus-15b/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/ultralm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/src/alpaca_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.371686 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 11:38:24.000000 alpaca_eval-0.2.6/src/alpaca_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:38:24.387688 alpaca_eval-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/tests/test_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/tests/test_decoders_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-25 11:37:55.000000 alpaca_eval-0.2.6/tests/test_pairwise_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.234441 alpaca_eval-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    67506 2023-07-31 02:10:28.234441 alpaca_eval-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66684 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.194441 alpaca_eval-0.2.7/example/
+-rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/example/outputs.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 02:10:28.234441 alpaca_eval-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.182441 alpaca_eval-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.198441 alpaca_eval-0.2.7/src/alpaca_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 02:10:11.000000 alpaca_eval-0.2.7/src/alpaca_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.202441 alpaca_eval-0.2.7/src/alpaca_eval/annotators/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28587 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/annotators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.202441 alpaca_eval-0.2.7/src/alpaca_eval/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12710 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/replicate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.202441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.202441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.206441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.206441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/test/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.186441 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    23982 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.194441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baichuan-13b-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baize-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baize-v2-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/chatglm2-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/claude-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/claude-2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/cohere-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-33b-api/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-33b-api/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v2-w-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v3.1-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v3.1-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat8192-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/opencoderplus-15b/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/ultralm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.234441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b-v1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b-v1.2/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.202441 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    67506 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.234441 alpaca_eval-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/tests/test_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/tests/test_decoders_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.2.6/LICENSE` & `alpaca_eval-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/PKG-INFO` & `alpaca_eval-0.2.7/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alpaca_eval
-Version: 0.2.6
+Name: alpaca-eval
+Version: 0.2.7
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -1128,17 +1128,15 @@
 used as replacement for human evaluation in important settings, such as to decide whether a model is ready to be
 deployed.
 Those can broadly be clustered into 3 categories:
 
 1. **Instructions might not be representative of real-usage**:  the AlpacaEval set contains examples from a variety of
    datasets ([self-instruct](https://github.com/yizhongw/self-instruct),
    [open-assistant](https://huggingface.co/datasets/OpenAssistant/oasst1/viewer/OpenAssistant--oasst1/validation), [vicuna](https://lmsys.org/blog/2023-03-30-vicuna/), [koala](https://github.com/arnav-gudibande/koala-test-set), [hh-rlhf](https://huggingface.co/datasets/Anthropic/hh-rlhf/viewer/Anthropic--hh-rlhf/test))
-   which might not be representative of real-usage and advanced applications of better models like GPT4. As a
-   result, the gap between the top and the rest of the AlpacaEval leaderboard is likely smaller than it would be on more
-   complex instructions. See for
+   which might not be representative of real-usage and advanced applications of better models like GPT4. This likely makes the best closed models (GPT4 / Claude / ChatGPT / ...) seem more similar to the open models than what they are. Indeed, those closed models seem to be pretrained/finetuned on much more diverse data. See for
    example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-open-source-models-on-slightly-harder-tasks-aa0395c31610)
    for preliminary results on more complex instructions.
    Note, however, that in [AlpacaFarm](https://arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation set
    are highly correlated (0.97 R2) with win-rates on instructions from user interactions with the Alpaca Demo.
    Furthermore, the AlpacaEval leaderboard shows larger
    gap between the open models and OpenAI models than other leaderboards (
    e.g. [lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.6 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.7 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -668,21 +668,22 @@
 contains examples from a variety of datasets ([self-instruct](https://
 github.com/yizhongw/self-instruct), [open-assistant](https://huggingface.co/
 datasets/OpenAssistant/oasst1/viewer/OpenAssistant--oasst1/validation),
 [vicuna](https://lmsys.org/blog/2023-03-30-vicuna/), [koala](https://
 github.com/arnav-gudibande/koala-test-set), [hh-rlhf](https://huggingface.co/
 datasets/Anthropic/hh-rlhf/viewer/Anthropic--hh-rlhf/test)) which might not be
 representative of real-usage and advanced applications of better models like
-GPT4. As a result, the gap between the top and the rest of the AlpacaEval
-leaderboard is likely smaller than it would be on more complex instructions.
-See for example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-
-open-source-models-on-slightly-harder-tasks-aa0395c31610) for preliminary
-results on more complex instructions. Note, however, that in [AlpacaFarm]
-(https://arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation
-set are highly correlated (0.97 R2) with win-rates on instructions from user
+GPT4. This likely makes the best closed models (GPT4 / Claude / ChatGPT / ...)
+seem more similar to the open models than what they are. Indeed, those closed
+models seem to be pretrained/finetuned on much more diverse data. See for
+example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-open-
+source-models-on-slightly-harder-tasks-aa0395c31610) for preliminary results on
+more complex instructions. Note, however, that in [AlpacaFarm](https://
+arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation set are
+highly correlated (0.97 R2) with win-rates on instructions from user
 interactions with the Alpaca Demo. Furthermore, the AlpacaEval leaderboard
 shows larger gap between the open models and OpenAI models than other
 leaderboards ( e.g. [lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)). 2.
 **Biases of automatic annotators**: the automatic annotators seem to have
 implicit biases. In particular, we found that they tend to prefer longer
 outputs and outputs that contain lists (e.g. 0.68 / 0.69 for `alpaca_eval_gpt4`
 and 0.62 / 0.58 for `claude`). Although we found that humans have similar
```

### Comparing `alpaca_eval-0.2.6/README.md` & `alpaca_eval-0.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1105,17 +1105,15 @@
 used as replacement for human evaluation in important settings, such as to decide whether a model is ready to be
 deployed.
 Those can broadly be clustered into 3 categories:
 
 1. **Instructions might not be representative of real-usage**:  the AlpacaEval set contains examples from a variety of
    datasets ([self-instruct](https://github.com/yizhongw/self-instruct),
    [open-assistant](https://huggingface.co/datasets/OpenAssistant/oasst1/viewer/OpenAssistant--oasst1/validation), [vicuna](https://lmsys.org/blog/2023-03-30-vicuna/), [koala](https://github.com/arnav-gudibande/koala-test-set), [hh-rlhf](https://huggingface.co/datasets/Anthropic/hh-rlhf/viewer/Anthropic--hh-rlhf/test))
-   which might not be representative of real-usage and advanced applications of better models like GPT4. As a
-   result, the gap between the top and the rest of the AlpacaEval leaderboard is likely smaller than it would be on more
-   complex instructions. See for
+   which might not be representative of real-usage and advanced applications of better models like GPT4. This likely makes the best closed models (GPT4 / Claude / ChatGPT / ...) seem more similar to the open models than what they are. Indeed, those closed models seem to be pretrained/finetuned on much more diverse data. See for
    example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-open-source-models-on-slightly-harder-tasks-aa0395c31610)
    for preliminary results on more complex instructions.
    Note, however, that in [AlpacaFarm](https://arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation set
    are highly correlated (0.97 R2) with win-rates on instructions from user interactions with the Alpaca Demo.
    Furthermore, the AlpacaEval leaderboard shows larger
    gap between the open models and OpenAI models than other leaderboards (
    e.g. [lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)).
```

#### html2text {}

```diff
@@ -657,21 +657,22 @@
 contains examples from a variety of datasets ([self-instruct](https://
 github.com/yizhongw/self-instruct), [open-assistant](https://huggingface.co/
 datasets/OpenAssistant/oasst1/viewer/OpenAssistant--oasst1/validation),
 [vicuna](https://lmsys.org/blog/2023-03-30-vicuna/), [koala](https://
 github.com/arnav-gudibande/koala-test-set), [hh-rlhf](https://huggingface.co/
 datasets/Anthropic/hh-rlhf/viewer/Anthropic--hh-rlhf/test)) which might not be
 representative of real-usage and advanced applications of better models like
-GPT4. As a result, the gap between the top and the rest of the AlpacaEval
-leaderboard is likely smaller than it would be on more complex instructions.
-See for example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-
-open-source-models-on-slightly-harder-tasks-aa0395c31610) for preliminary
-results on more complex instructions. Note, however, that in [AlpacaFarm]
-(https://arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation
-set are highly correlated (0.97 R2) with win-rates on instructions from user
+GPT4. This likely makes the best closed models (GPT4 / Claude / ChatGPT / ...)
+seem more similar to the open models than what they are. Indeed, those closed
+models seem to be pretrained/finetuned on much more diverse data. See for
+example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-open-
+source-models-on-slightly-harder-tasks-aa0395c31610) for preliminary results on
+more complex instructions. Note, however, that in [AlpacaFarm](https://
+arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation set are
+highly correlated (0.97 R2) with win-rates on instructions from user
 interactions with the Alpaca Demo. Furthermore, the AlpacaEval leaderboard
 shows larger gap between the open models and OpenAI models than other
 leaderboards ( e.g. [lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)). 2.
 **Biases of automatic annotators**: the automatic annotators seem to have
 implicit biases. In particular, we found that they tend to prefer longer
 outputs and outputs that contain lists (e.g. 0.68 / 0.69 for `alpaca_eval_gpt4`
 and 0.62 / 0.58 for `claude`). Although we found that humans have similar
```

### Comparing `alpaca_eval-0.2.6/example/outputs.json` & `alpaca_eval-0.2.7/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/setup.py` & `alpaca_eval-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/analyze.py` & `alpaca_eval-0.2.7/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/annotators/base.py` & `alpaca_eval-0.2.7/src/alpaca_eval/annotators/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,68 +102,76 @@
 
         self.annotators_config = self._initialize_annotators_config(annotators_config)
         self.annotators = self._initialize_annotators()
         self.df_annotations = None
 
     ### Abstract methods ###
 
+    #######################
     @property
-    @abc.abstractmethod
     def SingleAnnotator(self) -> Type["SingleAnnotator"]:
-        """Class to use for each single annotator."""
-        pass
+        """Class to use for each annotator."""
+        return SingleAnnotator
 
-    #######################
     @property
     def available_fields_to_format(self):
         """Fields that can be formatted in the prompt template."""
         return self.all_keys
 
     @property
     def annotation_key(self) -> str:
         """How to refer to the annotations, this will be the key for annotations in the output."""
         return "annotation"
 
     @property
-    def random_seed_key(self) -> list[str]:
+    def random_seed_keys(self) -> list[str]:
         """What key / column to seed on for the random generator."""
         return list(self.primary_keys)
 
     ### Public methods ###
     @property
     def annotator_name(self) -> str:
         return Path(self.annotators_config).parent.name
 
     def __call__(
         self,
         to_annotate: utils.AnyData,
+        chunksize: Optional[int] = 128,
         **decoding_kwargs,
     ) -> list[dict[str, Any]]:
         """Main function for annotating.
 
         Parameters
         ----------
         to_annotate : list of dict or dataframe
             Examples to annotate. Each dictionary (or row) should contain all of `self.primary_keys`.
 
+        chunksize : int, optional
+            The number of rows to annotate at once => ensures that if there is an error, you still get some annotations.
+
         **decoding_kwargs :
             Additional arguments to pass to `fn_completions`.
 
         Returns
         -------
         annotated : list of dict
             The annotated examples. Each dict will contain all of `self.primary_keys` and `self.annotation_key`.
         """
         if len(to_annotate) == 0:
             return []
 
-        df_to_annotate = self._preprocess(to_annotate)
-        df_annotated = self._annotate(df_to_annotate, **decoding_kwargs)
-        annotated = self._postprocess_and_store_(df_annotated, to_annotate)
-        return annotated
+        # note: not ideal potentially doing a lot of dataframe copies. But given that they should be small, ~ok
+        df_to_annotate = utils.convert_to_dataframe(to_annotate)
+        all_annotated = []
+        for df_chunk in utils.dataframe_chunk_generator(df_to_annotate, chunksize, tqdm_desc="Annotation chunk"):
+            curr_df_to_annotate = self._preprocess(df_chunk)
+            df_annotated = self._annotate(curr_df_to_annotate, **decoding_kwargs)
+            annotated = self._postprocess_and_store_(df_annotated, df_chunk)
+            all_annotated.extend(annotated)
+        return all_annotated
 
     #######################
 
     ### Private methods ###
     def _initialize_annotators_config(self, annotators_config):
         # setting it relative to the config directory
         annotators_config = self.base_dir / annotators_config
@@ -215,15 +223,15 @@
         # remove duplicates because you only need to annotate one of them
         df_to_annotate = df_to_annotate.drop_duplicates(subset=self.primary_keys)
 
         # set the annotater for each example
         df_to_annotate[self.annotator_column] = df_to_annotate.apply(
             lambda x: utils.random_seeded_choice(
                 # we add "annotator" at the beginning to not use the same seed for all tasks
-                seed="annotator" + "".join(x[self.random_seed_key]) + str(self.seed),
+                seed="annotator" + "".join(x[self.random_seed_keys]) + str(self.seed),
                 choices=list(self.annotators.keys()),
             ),
             axis=1,
         )
 
         if self.is_avoid_reannotations:
             df_to_annotate = self._apply_cached_annotations(df_to_annotate)
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.2.7/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         return SinglePairwiseAnnotator
 
     @property
     def annotation_key(self) -> str:
         return "preference"
 
     @property
-    def random_seed_key(self) -> list[str]:
+    def random_seed_keys(self) -> list[str]:
         return list(self.input_keys)
 
     def annotate_samples(
         self,
         all_outputs: utils.AnyData,
         keys_to_sample_output_2: Optional[Sequence] = None,
         is_unique_instructions: bool = True,
@@ -283,15 +283,15 @@
         if self.p_label_flip:
             logging.info(f"Adding random noise to the labels p_label_flip={self.p_label_flip}.")
             # if you have 25% change of flipping the label, you have 50% chance of selecting random label
             p_noise = self.p_label_flip * 2
             noisy_preference = df_to_annotate.apply(
                 # we add "noisy_label" at the beginning to use ~independent seeds between tasks
                 lambda x: utils.random_seeded_choice(  # seed on inputs for reproducibility
-                    seed="noisy_preference" + "".join(x[self.random_seed_key]) + str(self.seed),
+                    seed="noisy_preference" + "".join(x[self.random_seed_keys]) + str(self.seed),
                     choices=[np.nan, 1, 2],
                     weights=[1 - p_noise, self.p_label_flip, self.p_label_flip],
                 ),
                 axis=1,
             )
             df_to_annotate["is_noisy_label"] = ~noisy_preference.isna()
             # keeps previously annotated examples when you did not add noise
@@ -327,15 +327,15 @@
             "A helper class for a single auto annotator.",
             "A helper class for a single pairwise auto annotator.",
         )
         + """
     is_randomize_output_order : bool
         Whether to randomize output_1, output_2 when formatting.
         
-    random_seed_key : str
+    random_seed_keys : str
         The column to use to seed the randomization of output_1, output_2.
     """
     )
 
     def __init__(
         self,
         *args,
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.2.7/src/alpaca_eval/completion_parsers.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 from typing import Any
 
 import numpy as np
 
 from . import utils
 
-__all__ = ["regex_parser", "lmsys_parser", "ranking_parser", "json_parser", "eval_parser"]
+__all__ = ["regex_parser", "lmsys_parser", "ranking_parser", "json_parser", "eval_parser", "pipeline_meta_parser"]
 
 
 def regex_parser(completion: str, outputs_to_match: dict[str, Any]) -> list[Any]:
     r"""Parse a single batch of completions, by returning a sequence of keys in the order in which outputs_to_match
     was matched.
 
     Parameters
@@ -161,7 +161,75 @@
     >>> eval_parser("[True,1,'False']")
     [True, 1, 'False']
     """
     evaluated_completion = ast.literal_eval(completion)
     if not isinstance(evaluated_completion, list):
         evaluated_completion = [evaluated_completion]
     return evaluated_completion
+
+
+def replace_parser(completion: str, replacer: dict, default_replacer: Any = "auto") -> list[str]:
+    """Parser that replaces part of the completion using a dictionary. This is useful if it's more natural for a
+    prompt to ask a completion that is different from the one you want to store.
+
+    Parameters
+    ----------
+    completion : str
+        Output from the model to parse.
+
+    replacer : dict
+        Dictionary with keys that are the substring of the completion that you want to replace and values that are the
+        replacements.
+
+    default_replacer : any, optional
+        If a key is not found in `replacer`, use this value instead. If "auto" then use the key itself.
+
+    Examples
+    --------
+    >>> replace_parser("True", replacer={"True": 1})
+    [1]
+    """
+    return [replacer.get(completion, completion if default_replacer == "auto" else default_replacer)]
+
+
+def pipeline_meta_parser(
+    completion: str, parsers_to_kwargs: dict[str, dict], is_squeeze: bool = True, _depth=0
+) -> list[Any]:
+    r"""Applies a list of parsers in sequence to a completion.
+
+    Parameters
+    ----------
+    completion : str
+        The completion to parse.
+
+    parsers_to_kwargs : dictionary of str to dict
+        A dictionary mapping parser functions to kwargs to pass to them. The parsing functions will be applied in the
+        order they are given.
+
+    is_squeeze : bool, optional
+        If True, will squeeze the output of each parser if it's a singleton.
+
+    Examples
+    --------
+    >>> completion = '{"ex": "...", "rank": [{"model": "model_1", "rank": 1}, {"model": "model_2", "rank": 2}]}'
+    >>> parsers_to_kwargs = {"json_parser": {"annotation_key": "rank"}, "ranking_parser": {}}
+    >>> pipeline_meta_parser(completion, parsers_to_kwargs)
+    [1]
+    """
+    all_parsers = list(parsers_to_kwargs.keys())
+    all_kwargs = list(parsers_to_kwargs.values())
+
+    out = globals()[all_parsers[0]](completion, **all_kwargs[0])
+    rest_of_parsers_to_kwargs = dict(zip(all_parsers[1:], all_kwargs[1:]))
+    if len(rest_of_parsers_to_kwargs) > 0:
+        out = [
+            pipeline_meta_parser(
+                o, parsers_to_kwargs=rest_of_parsers_to_kwargs, is_squeeze=is_squeeze, _depth=_depth + 1
+            )
+            for o in out
+        ]
+
+    if is_squeeze and len(out) == 1 and _depth != 0:
+        assert isinstance(out, list)
+        out = out[0]
+
+    return out
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/constants.py` & `alpaca_eval-0.2.7/src/alpaca_eval/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.2.7/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.2.7/src/alpaca_eval/decoders/anthropic.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.2.7/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.2.7/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def huggingface_api_completions(
     prompts: Sequence[str],
     model_name: str,
     gpu: bool = False,
     do_sample: bool = False,
-    num_procs: int = 8,
+    num_procs: int = 1,
     **kwargs,
 ) -> dict[str, list]:
     """Decode with the API from hugging face hub.
 
     Parameters
     ----------
     prompts : list of str
@@ -92,15 +92,15 @@
             error = output["error"]
             if "Rate limit reached" in output["error"]:
                 logging.warning(f"Rate limit reached... Trying again in {waiting_time} seconds. Full error: {error}")
                 time.sleep(waiting_time)
             elif "Input validation error" in error and "max_new_tokens" in error:
                 params["max_new_tokens"] = int(params["max_new_tokens"] * 0.8)
                 logging.warning(
-                    f"`max_new_tokens` too large. Reducing target length to {params['max_tokens']}, " f"Retrying..."
+                    f"`max_new_tokens` too large. Reducing target length to {params['max_new_tokens']}, " f"Retrying..."
                 )
                 if params["max_new_tokens"] == 0:
                     raise ValueError(f"Error in inference. Full error: {error}")
             else:
                 raise ValueError(f"Error in inference. Full error: {error}")
         else:
             return output[0]
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.2.7/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.2.7/src/alpaca_eval/decoders/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,20 +195,16 @@
                     assert choice.message.role == "assistant"
                     if choice.message.content == "":
                         choice["text"] = " "  # annoying doesn't allow empty string
                     else:
                         choice["text"] = choice.message.content
 
                     if choice.message.get("function_call"):
-                        # currently we only use function calls to get a JSON object
-                        # => overwrite text with the JSON object. In the future, we could
-                        # allow actual function calls
-                        all_args = json.loads(choice.message.function_call.arguments)
-                        assert len(all_args) == 1
-                        choice["text"] = all_args[list(all_args.keys())[0]]
+                        # currently we only use function calls to get a JSON object => return raw text of json
+                        choice["text"] = choice.message.function_call.arguments
 
             else:
                 completion_batch = openai.Completion.create(prompt=prompt_batch, **curr_kwargs)
                 choices = completion_batch.choices
 
             for choice in choices:
                 choice["total_tokens"] = completion_batch.usage.total_tokens / len(prompt_batch)
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/decoders/replicate.py` & `alpaca_eval-0.2.7/src/alpaca_eval/decoders/replicate.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 __all__ = ["replicate_completions"]
 
 
 def replicate_completions(
     prompts: Sequence[str],
     model_name: str,
-    num_procs: int = 16,
+    num_procs: int = 32,
     **decoding_kwargs,
 ) -> dict[str, list]:
     r"""Get completions using a model hosted on https://replicate.com/.
 
     Parameters
     ----------
     prompts : list of str
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -22,9 +22,14 @@
                   model:
                     type: "string"
                     description: "The name of the model"
                   rank:
                     type: "number"
                     description: "Order of preference of the model, 1 has the best output"
         "required": [ "ordered_models" ]
-  fn_completion_parser: "ranking_parser"
+  fn_completion_parser: "pipeline_meta_parser"
+  completion_parser_kwargs:
+      parsers_to_kwargs:
+        json_parser:
+          annotation_key: "ordered_models"
+        ranking_parser: {}
   batch_size: 1
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base,avg_length
-gpt4,95.27950310559004,0.716281440286153,minimal,12,805,761,32,1365
-claude-2,91.35572139303484,0.9897323784630048,minimal,1,804,734,69,1069
-vicuna-33b-v1.3,88.99253731343283,1.095692216068168,verified,5,804,713,86,1479
-claude,88.38509316770187,1.1144875403283188,minimal,9,805,707,89,1082
-openchat-v2-w-13b,87.1268656716418,1.1769197439396015,community,3,804,699,102,1566
-wizardlm-13b-v1.1,86.31840796019901,1.2063217831272972,community,4,804,692,108,1525
-chatgpt,86.08695652173914,1.2110077772660273,minimal,6,805,690,109,811
-llama-2-70b-chat-hf,85.136815920398,1.253783670416838,minimal,1,804,684,119,1451
-openchat-v2-13b,84.96894409937889,1.2572979835605944,community,2,805,683,120,1564
-vicuna-13b-v1.3,82.11180124223603,1.348769957803504,verified,2,805,660,143,1132
-llama-2-13b-chat-hf,81.09452736318407,1.3817573087734825,minimal,0,804,652,152,1513
-openchat-13b,80.8695652173913,1.3843738653129234,community,2,805,650,153,1632
-ultralm-13b,80.63511830635119,1.3939556917204066,community,1,803,647,155,1087
-openchat8192-13b,79.53980099502488,1.4222439886269744,community,1,804,639,164,1664
-opencoderplus-15b,78.69565217391305,1.440029529188432,community,3,805,632,170,1628
-vicuna-7b-v1.3,76.8414481897628,1.487520320531845,verified,3,801,614,184,1110
-wizardlm-13b,75.31094527363184,1.5101858292160824,minimal,9,804,601,194,985
-airoboros-65b,73.91304347826086,1.5285333061227804,community,16,805,587,202,1512
-airoboros-33b,73.29192546583852,1.55290318216736,community,6,805,587,212,1514
-guanaco-65b,71.80124223602485,1.586912361158523,minimal,0,805,578,227,1249
-llama-2-7b-chat-hf,71.36645962732919,1.593038654706019,minimal,1,805,574,230,1479
-vicuna-13b,70.43478260869566,1.6069688407799696,minimal,2,805,566,237,1037
-baize-v2-13b,66.95652173913044,1.6565358231309506,community,2,805,538,265,930
-oasst-rlhf-llama-33b,66.52173913043478,1.6608288428292477,minimal,3,805,534,268,1079
-minotaur-13b,66.02484472049689,1.6645545328264226,community,5,805,529,271,881
-guanaco-33b,65.96273291925466,1.67108537053247,verified,0,805,531,274,1311
-nous-hermes-13b,65.46583850931677,1.669962276077284,verified,6,805,524,275,844
-vicuna-7b,64.40993788819875,1.6851107260487883,verified,3,805,517,285,1044
-baize-v2-7b,63.85093167701863,1.6945981855442178,community,0,805,514,291,1127
-oasst-sft-llama-33b,54.96894409937888,1.7402667933686875,verified,13,805,436,356,748
-guanaco-13b,52.60869565217391,1.7576690299699242,verified,3,805,422,380,1774
-text_davinci_003,50.0,0.0,minimal,805,805,0,0,307
-chatglm2-6b,47.12858926342072,1.7593143221324448,community,5,801,375,421,1027
-guanaco-7b,46.58385093167702,1.7570464905413992,verified,2,805,374,429,1364
-falcon-40b-instruct,45.71428571428572,1.7524717060805597,minimal,4,805,366,435,662
-alpaca-farm-ppo-sim-gpt4-20k,44.099378881987576,1.7399772578861137,verified,10,805,350,445,511
-pythia-12b-mix-sft,41.86335403726708,1.737637146007538,verified,2,805,336,467,913
-alpaca-farm-ppo-human,41.24223602484472,1.7271813123250834,minimal,8,805,328,469,803
-cohere-chat,29.565217391304348,1.5949050483247118,community,12,805,232,561,779
-cohere,28.385093167701864,1.5717547121761728,community,15,805,221,569,682
-alpaca-7b,26.459627329192543,1.535711469748,minimal,16,805,205,584,396
-oasst-sft-pythia-12b,25.962732919254663,1.5261079289535309,verified,16,805,201,588,726
-falcon-7b-instruct,23.60248447204969,1.4898235369056625,verified,6,805,187,612,478
-baichuan-13b-chat,21.801242236024844,1.4495247592518703,community,5,805,173,627,1727
-text_davinci_001,15.17412935323383,1.235107892276849,minimal,20,804,112,672,296
+,win_rate,standard_error,n_wins,n_wins_base,n_draws,n_total,mode,avg_length
+gpt4,95.27950310559004,0.716281440286153,761,32,12,805,minimal,1365
+llama-2-70b-chat-hf,92.66169154228857,0.911762258320568,743,57,4,804,minimal,1790
+claude-2,91.35572139303484,0.9897323784630048,734,69,1,804,minimal,1069
+openchat-v3.1-13b,89.49004975124379,1.076875474505156,718,83,3,804,community,1484
+chatgpt,89.36567164179104,1.0789487022114888,716,83,5,804,minimal,827
+wizardlm-13b-v1.2,89.1656288916563,1.0904254662753898,714,85,4,803,community,1635
+vicuna-33b-v1.3,88.99253731343283,1.095692216068168,713,86,5,804,verified,1479
+claude,88.38509316770187,1.1144875403283188,707,89,9,805,minimal,1082
+openchat-v2-w-13b,87.1268656716418,1.1769197439396015,699,102,3,804,community,1566
+wizardlm-13b-v1.1,86.31840796019901,1.2063217831272972,692,108,4,804,community,1525
+openchat-v2-13b,84.96894409937889,1.2572979835605944,683,120,2,805,community,1564
+vicuna-13b-v1.3,82.11180124223603,1.348769957803504,660,143,2,805,verified,1132
+llama-2-13b-chat-hf,81.09452736318407,1.3817573087734825,652,152,0,804,minimal,1513
+openchat-13b,80.8695652173913,1.3843738653129234,650,153,2,805,community,1632
+ultralm-13b,80.63511830635119,1.3939556917204066,647,155,1,803,community,1087
+openchat8192-13b,79.53980099502488,1.4222439886269744,639,164,1,804,community,1664
+opencoderplus-15b,78.69565217391305,1.440029529188432,632,170,3,805,community,1628
+vicuna-7b-v1.3,76.8414481897628,1.487520320531845,614,184,3,801,verified,1110
+wizardlm-13b,75.31094527363184,1.5101858292160824,601,194,9,804,minimal,985
+airoboros-65b,73.91304347826086,1.5285333061227804,587,202,16,805,community,1512
+airoboros-33b,73.29192546583852,1.55290318216736,587,212,6,805,community,1514
+guanaco-65b,71.80124223602485,1.586912361158523,578,227,0,805,minimal,1249
+llama-2-7b-chat-hf,71.36645962732919,1.593038654706019,574,230,1,805,minimal,1479
+vicuna-13b,70.43478260869566,1.6069688407799696,566,237,2,805,minimal,1037
+baize-v2-13b,66.95652173913044,1.6565358231309506,538,265,2,805,community,930
+oasst-rlhf-llama-33b,66.52173913043478,1.6608288428292477,534,268,3,805,minimal,1079
+minotaur-13b,66.02484472049689,1.6645545328264226,529,271,5,805,community,881
+guanaco-33b,65.96273291925466,1.67108537053247,531,274,0,805,verified,1311
+nous-hermes-13b,65.46583850931677,1.669962276077284,524,275,6,805,verified,844
+vicuna-7b,64.40993788819875,1.6851107260487883,517,285,3,805,verified,1044
+baize-v2-7b,63.85093167701863,1.6945981855442178,514,291,0,805,community,1127
+oasst-sft-llama-33b,54.96894409937888,1.7402667933686875,436,356,13,805,verified,748
+guanaco-13b,52.60869565217391,1.7576690299699242,422,380,3,805,verified,1774
+text_davinci_003,50.0,0.0,0,0,805,805,minimal,307
+chatglm2-6b,47.12858926342072,1.7593143221324448,375,421,5,801,community,1027
+guanaco-7b,46.58385093167702,1.7570464905413992,374,429,2,805,verified,1364
+falcon-40b-instruct,45.71428571428572,1.7524717060805597,366,435,4,805,minimal,662
+alpaca-farm-ppo-sim-gpt4-20k,44.099378881987576,1.7399772578861137,350,445,10,805,verified,511
+pythia-12b-mix-sft,41.86335403726708,1.737637146007538,336,467,2,805,verified,913
+alpaca-farm-ppo-human,41.24223602484472,1.7271813123250834,328,469,8,805,minimal,803
+cohere-chat,29.565217391304348,1.5949050483247118,232,561,12,805,community,779
+cohere,28.385093167701864,1.5717547121761728,221,569,15,805,community,682
+alpaca-7b,26.459627329192543,1.535711469748,205,584,16,805,minimal,396
+oasst-sft-pythia-12b,25.962732919254663,1.5261079289535309,201,588,16,805,verified,726
+falcon-7b-instruct,23.60248447204969,1.4898235369056625,187,612,6,805,verified,478
+baichuan-13b-chat,21.801242236024844,1.4495247592518703,173,627,5,805,community,1727
+text_davinci_001,15.17412935323383,1.235107892276849,112,672,20,804,minimal,296
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv` & `alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base,output_length,avg_length
 gpt4,77.01863354037268,1.46803688292698,minimal,12,805,614,179,,1365
 claude,75.83850931677019,1.4981004247868313,minimal,9,805,606,190,,1082
+llama-2-70b-chat-hf,72.91925465838509,1.5622590981080728,minimal,4,805,585,216,,1790
 vicuna-33b-v1.3,72.36024844720497,1.5710737760483915,verified,5,805,580,220,,1479
 claude-2,71.98757763975155,1.5824915958976835,minimal,1,805,579,225,1069.0,1069
 chatgpt,67.70186335403726,1.642111587090117,minimal,6,805,542,257,,811
 vicuna-13b-v1.3,66.2111801242236,1.6657907370589309,verified,2,805,532,271,,1132
-llama-2-70b-chat-hf,66.14906832298136,1.6676994320973642,minimal,1,805,532,272,,1451
 wizardlm-13b,66.14906832298136,1.6584088766540706,minimal,9,805,528,268,,985
 vicuna-13b,63.22981366459627,1.698243477332765,minimal,2,805,508,295,,1037
 guanaco-65b,62.60869565217392,1.7063755171155923,minimal,0,805,504,301,,1249
 vicuna-7b-v1.3,62.54658385093168,1.7035470981976453,verified,3,805,502,300,,1110
 nous-hermes-13b,60.86956521739131,1.7144465955143962,verified,6,805,487,312,,844
 guanaco-33b,57.88819875776397,1.7412811662531051,verified,0,805,466,339,,1311
 vicuna-7b,57.329192546583855,1.7409917994657298,verified,3,805,460,342,,1044
 oasst-rlhf-llama-33b,57.329192546583855,1.7409917994657302,minimal,3,805,460,342,,1079
-llama-2-13b-chat-hf,56.149068322981364,1.7499783078823692,minimal,0,805,452,353,,1513
+llama-2-13b-chat-hf,56.14906832298136,1.7499783078823692,minimal,0,805,452,353,,1513
 guanaco-13b,53.36239103362392,1.7582560332920765,verified,3,803,427,373,,1774
 llama-2-7b-chat-hf,51.98757763975155,1.7608738025727095,minimal,1,805,418,386,,1479
 oasst-sft-llama-33b,51.24223602484472,1.748518981999294,verified,13,805,406,386,,748
 text_davinci_003,50.0,0.0,minimal,805,805,0,0,,307
 alpaca-farm-ppo-sim-gpt4-20k,48.19875776397515,1.7512254507446705,verified,10,805,383,412,,511
 guanaco-7b,47.5776397515528,1.7590989434689512,verified,2,805,382,421,,1364
 falcon-40b-instruct,46.70807453416149,1.7551420072945083,minimal,4,805,374,427,,662
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/main.py` & `alpaca_eval-0.2.7/src/alpaca_eval/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,17 +83,17 @@
         should take a sequence of preferences (0 for draw, 1 for base win, 2 when the model to compare wins) and return
         a dictionary of metrics and the key by which to sort the leaderboard.
 
     sort_by : str, optional
         The key by which to sort the leaderboard.
 
     is_cache_leaderboard : bool, optional
-        Whether to save the result leaderboard to `precomputed_leaderboard`. If None we save only if max_instances.
-        A preferred way of adding models to the leaderboard is to set `precomputed_leaderboard` to the previously
-        saved leaderboard at `<output_path>/leaderboard.csv`.
+        Whether to save the result leaderboard to `precomputed_leaderboard`. If None we save only if max_instances
+        not None. A preferred way of adding models to the leaderboard is to set `precomputed_leaderboard` to the
+        previously saved leaderboard at `<output_path>/leaderboard.csv`.
 
     max_instances : int, optional
         The maximum number of instances to annotate. Useful for testing.
 
     annotation_kwargs : dict, optional
         Additional arguments to pass to `PairwiseAnnotator.annotate_head2head`.
 
@@ -185,14 +185,16 @@
     model_configs: Union[AnyPath, dict],
     reference_model_configs: Optional[Union[AnyPath, dict]] = None,
     evaluation_dataset: Union[AnyPath, AnyData, Callable] = constants.ALPACAEVAL_REFERENCE_OUTPUTS,
     annotators_config: AnyPath = DEFAULT_CONFIGS,
     output_path: AnyPath = "auto",
     max_instances: int = None,
     is_strip_output: bool = True,
+    is_load_outputs: bool = True,
+    chunksize: int = 64,
     **kwargs,
 ):
     """Evaluate a model from HuggingFace or an API provider. This is a wrapper around `evaluate` which includes
     generating from
     a desired model.
 
     Parameters
@@ -222,60 +224,105 @@
 
     max_instances : int, optional
         Maximum number of instances to generate and evaluate. If None, we evaluate all instances.
 
     is_strip_output : bool, optional
         Whether to strip trailing and leading whitespaces from the outputs.
 
+    is_load_outputs : bool, optional
+        Whether to try to load outputs from the output path. If True and outputs exist we only generate outputs for
+        instructions that don't have outputs yet.
+
+    chunksize : int, optional
+        Number of instances to generate before saving. If None, we save after all generations.
+
     kwargs:
         Other kwargs to `evaluate`
     """
-    evaluation_dataset = utils.load_or_convert_to_dataframe(evaluation_dataset)
+    df_dataset = utils.load_or_convert_to_dataframe(evaluation_dataset)
+
+    if chunksize is not None and not is_load_outputs:
+        logging.info("`is_load_outputs` has to be true to use chunksize. Setting it to True.")
+        is_load_outputs = True
+
+    if chunksize is not None and max_instances is not None:
+        logging.info("cannot use `chunksize` with max_instances. Setting `chunksize` to None.")
+        chunksize = None
 
     model_configs = utils.load_configs(model_configs, relative_to=constants.MODELS_CONFIG_DIR)
     if reference_model_configs is not None:
         reference_model_configs = utils.load_configs(reference_model_configs, relative_to=constants.MODELS_CONFIG_DIR)
 
-    def get_completions(configs):
-        columns_to_keep = ["dataset", "instruction", "output"]
-        columns_to_keep = [c for c in columns_to_keep if c in evaluation_dataset.columns]
-        curr_outputs = evaluation_dataset.copy()[columns_to_keep]
-        if max_instances is not None:
-            curr_outputs = curr_outputs.iloc[:max_instances]
+    if output_path == "auto":
+        output_path = Path("results") / list(model_configs.keys())[0]
+    if output_path is not None:
+        output_path = Path(output_path)
+        output_path.mkdir(exist_ok=True, parents=True)
+
+    def get_completions(configs, df: pd.DataFrame, old_output_path: Optional[Path] = None):
+        columns_to_keep = ["dataset", "instruction", "output", "generator"]
+        columns_to_keep = [c for c in columns_to_keep if c in df.columns]
+        curr_outputs = df[columns_to_keep].copy()
+        is_loading_old_outputs = old_output_path is not None and old_output_path.exists()
         assert len(configs) == 1
         generator = list(configs.keys())[0]
         configs = list(configs.values())[0]
-        prompts, _ = utils.make_prompts(
-            curr_outputs,
-            template=utils.read_or_return(constants.MODELS_CONFIG_DIR / configs["prompt_template"]),
-        )
-        fn_completions = decoders.get_fn_completions(configs["fn_completions"])
-        completions = fn_completions(prompts=prompts, **configs["completions_kwargs"])["completions"]
-        if is_strip_output:
-            completions = [c.strip() for c in completions]
-        curr_outputs["output"] = completions
-        curr_outputs["generator"] = generator
+
+        if is_loading_old_outputs:
+            logging.info(f"Loading outputs from {old_output_path}")
+            old_outputs = utils.load_or_convert_to_dataframe(old_output_path)
+            # select only rows in curr_outputs that have "instruction" that are not in old_outputs
+            idx_found_old_outputs = curr_outputs["instruction"].isin(old_outputs["instruction"])
+            curr_outputs = curr_outputs[~idx_found_old_outputs]
+            assert (old_outputs["generator"] == generator).all()
+
+        if max_instances is not None:
+            curr_outputs = curr_outputs.iloc[:max_instances]
+
+        if len(curr_outputs) > 0:
+            prompts, _ = utils.make_prompts(
+                curr_outputs,
+                template=utils.read_or_return(constants.MODELS_CONFIG_DIR / configs["prompt_template"]),
+            )
+            fn_completions = decoders.get_fn_completions(configs["fn_completions"])
+            completions = fn_completions(prompts=prompts, **configs["completions_kwargs"])["completions"]
+            if is_strip_output:
+                completions = [c.strip() for c in completions]
+            curr_outputs["output"] = completions
+            curr_outputs["generator"] = generator
+
+        if is_loading_old_outputs:
+            curr_outputs = pd.concat([old_outputs, curr_outputs], axis=0)
+
         return curr_outputs
 
-    model_outputs = get_completions(model_configs)
-    if reference_model_configs is None:
-        if "output" not in evaluation_dataset.columns:
-            raise ValueError("evaluation_dataset should have a column 'output' containing references outputs")
-        reference_outputs = evaluation_dataset.copy()
-    else:
-        reference_outputs = get_completions(reference_model_configs)
+    for df_chunk in utils.dataframe_chunk_generator(
+        df_dataset, chunksize=chunksize, tqdm_desc="Chunking for generation"
+    ):
+        if is_load_outputs and output_path is not None:
+            model_outputs = get_completions(
+                model_configs, df=df_chunk, old_output_path=output_path / "model_outputs.json"
+            )
+        else:
+            model_outputs = get_completions(model_configs, df=df_chunk)
 
-    if output_path == "auto":
-        output_path = Path("results") / (model_outputs["generator"].iloc[0])
+        if reference_model_configs is None:
+            if "output" not in df_chunk.columns:
+                raise ValueError("evaluation_dataset should have a column 'output' containing references outputs")
+            reference_outputs = df_dataset.copy()
+        else:
+            reference_outputs = get_completions(
+                reference_model_configs,
+                df=df_chunk,
+                old_output_path=output_path / "reference_outputs.json",
+            )
 
-    if output_path is not None:
-        output_path = Path(output_path)
-        output_path.mkdir(exist_ok=True, parents=True)
-        model_outputs.to_json(output_path / "model_outputs.json", orient="records", indent=2)
-        reference_outputs.to_json(output_path / "reference_outputs.json", orient="records", indent=2)
+        if output_path is not None:
+            model_outputs.to_json(output_path / "model_outputs.json", orient="records", indent=2)
+            reference_outputs.to_json(output_path / "reference_outputs.json", orient="records", indent=2)
 
     return evaluate(
         model_outputs=model_outputs,
         reference_outputs=reference_outputs,
         annotators_config=annotators_config,
         output_path=output_path,
         max_instances=max_instances,
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/metrics.py` & `alpaca_eval-0.2.7/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt` & `alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/plotting.py` & `alpaca_eval-0.2.7/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/processors.py` & `alpaca_eval-0.2.7/src/alpaca_eval/processors.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval/utils.py` & `alpaca_eval-0.2.7/src/alpaca_eval/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pathlib import Path
 from typing import Any, Callable, Optional, Sequence, Union
 
 import datasets
 import numpy as np
 import pandas as pd
 import pkg_resources
+import tqdm
 import yaml
 
 from . import constants
 
 # don't load from utils to avoid unnecessary dependencies
 AnyPath = Union[str, os.PathLike, pathlib.Path]
 AnyData = Union[Sequence[dict[str, Any]], pd.DataFrame, datasets.Dataset]
@@ -397,14 +398,15 @@
                 if name is not None:
                     output_path = Path("results") / name
                 else:
                     output_path = "."
     if output_path is not None:
         output_path = Path(output_path)
         output_path.mkdir(exist_ok=True, parents=True)
+    return output_path
 
 
 def print_leaderboard(df_leaderboard, leaderboard_mode, cols_to_print, current_name=None):
     cols_to_print = list(cols_to_print)
 
     if leaderboard_mode is not None:
         if "mode" in df_leaderboard.columns:
@@ -441,7 +443,41 @@
     elif hasattr(module, func_name):
         raise AttributeError(
             f"The function {func_name} is not allowed,add it to __all__ if needed."
             f" Available functions: {module.__all__}"
         )
     else:
         raise AttributeError(f"The function {func_name} does not exist. Available functions: {module.__all__}")
+
+
+def dataframe_chunk_generator(df: pd.DataFrame, chunksize: Optional[int] = None, tqdm_desc: Optional[str] = None):
+    """Generator that yields chunks of a dataframe.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        The dataframe to split into chunks.
+
+    chunksize : int, optional
+        The size of the chunks. If None, the chunksize will be the length of the dataframe.
+
+    tqdm_desc : bool, optional
+        Description to display in the tqdm progress bar. If None, no progress bar will be displayed.
+    """
+    if chunksize is None:
+        chunksize = max(1, len(df))
+
+    iterator = range(0, len(df), chunksize)
+
+    if tqdm_desc is not None:
+        iterator = tqdm.tqdm(iterator, desc=tqdm_desc)
+
+    n_iter = len(df) // chunksize
+
+    for i in iterator:
+        df_chunk = df.iloc[i : i + chunksize]
+
+        # if many iterations then better to copy the dataframe to avoid memory issues
+        if n_iter > 1:
+            df_chunk = df_chunk.copy()
+
+        yield df_chunk
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alpaca-eval
-Version: 0.2.6
+Name: alpaca_eval
+Version: 0.2.7
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -1128,17 +1128,15 @@
 used as replacement for human evaluation in important settings, such as to decide whether a model is ready to be
 deployed.
 Those can broadly be clustered into 3 categories:
 
 1. **Instructions might not be representative of real-usage**:  the AlpacaEval set contains examples from a variety of
    datasets ([self-instruct](https://github.com/yizhongw/self-instruct),
    [open-assistant](https://huggingface.co/datasets/OpenAssistant/oasst1/viewer/OpenAssistant--oasst1/validation), [vicuna](https://lmsys.org/blog/2023-03-30-vicuna/), [koala](https://github.com/arnav-gudibande/koala-test-set), [hh-rlhf](https://huggingface.co/datasets/Anthropic/hh-rlhf/viewer/Anthropic--hh-rlhf/test))
-   which might not be representative of real-usage and advanced applications of better models like GPT4. As a
-   result, the gap between the top and the rest of the AlpacaEval leaderboard is likely smaller than it would be on more
-   complex instructions. See for
+   which might not be representative of real-usage and advanced applications of better models like GPT4. This likely makes the best closed models (GPT4 / Claude / ChatGPT / ...) seem more similar to the open models than what they are. Indeed, those closed models seem to be pretrained/finetuned on much more diverse data. See for
    example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-open-source-models-on-slightly-harder-tasks-aa0395c31610)
    for preliminary results on more complex instructions.
    Note, however, that in [AlpacaFarm](https://arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation set
    are highly correlated (0.97 R2) with win-rates on instructions from user interactions with the Alpaca Demo.
    Furthermore, the AlpacaEval leaderboard shows larger
    gap between the open models and OpenAI models than other leaderboards (
    e.g. [lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.6 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.7 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -668,21 +668,22 @@
 contains examples from a variety of datasets ([self-instruct](https://
 github.com/yizhongw/self-instruct), [open-assistant](https://huggingface.co/
 datasets/OpenAssistant/oasst1/viewer/OpenAssistant--oasst1/validation),
 [vicuna](https://lmsys.org/blog/2023-03-30-vicuna/), [koala](https://
 github.com/arnav-gudibande/koala-test-set), [hh-rlhf](https://huggingface.co/
 datasets/Anthropic/hh-rlhf/viewer/Anthropic--hh-rlhf/test)) which might not be
 representative of real-usage and advanced applications of better models like
-GPT4. As a result, the gap between the top and the rest of the AlpacaEval
-leaderboard is likely smaller than it would be on more complex instructions.
-See for example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-
-open-source-models-on-slightly-harder-tasks-aa0395c31610) for preliminary
-results on more complex instructions. Note, however, that in [AlpacaFarm]
-(https://arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation
-set are highly correlated (0.97 R2) with win-rates on instructions from user
+GPT4. This likely makes the best closed models (GPT4 / Claude / ChatGPT / ...)
+seem more similar to the open models than what they are. Indeed, those closed
+models seem to be pretrained/finetuned on much more diverse data. See for
+example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-open-
+source-models-on-slightly-harder-tasks-aa0395c31610) for preliminary results on
+more complex instructions. Note, however, that in [AlpacaFarm](https://
+arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation set are
+highly correlated (0.97 R2) with win-rates on instructions from user
 interactions with the Alpaca Demo. Furthermore, the AlpacaEval leaderboard
 shows larger gap between the open models and OpenAI models than other
 leaderboards ( e.g. [lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)). 2.
 **Biases of automatic annotators**: the automatic annotators seem to have
 implicit biases. In particular, we found that they tend to prefer longer
 outputs and outputs that contain lists (e.g. 0.68 / 0.69 for `alpaca_eval_gpt4`
 and 0.62 / 0.58 for `claude`). Although we found that humans have similar
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.2.7/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -101,23 +101,21 @@
 src/alpaca_eval/models_configs/cohere-chat/configs.yaml
 src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
 src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
 src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
 src/alpaca_eval/models_configs/gpt4/configs.yaml
 src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+src/alpaca_eval/models_configs/guanaco-33b-api/configs.yaml
 src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
 src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
 src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
-src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/configs.yaml
-src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/prompt.txt
-src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/configs.yaml
-src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/prompt.txt
+src/alpaca_eval/models_configs/llama-2-70b-chat-hf/prompt.txt
 src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
 src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
 src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
 src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
 src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
 src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
 src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
@@ -125,14 +123,15 @@
 src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
 src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
 src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
 src/alpaca_eval/models_configs/openchat-13b/configs.yaml
 src/alpaca_eval/models_configs/openchat-13b/prompt.txt
 src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
 src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
+src/alpaca_eval/models_configs/openchat-v3.1-13b/configs.yaml
 src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
 src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
 src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
 src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
 src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
 src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
 src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
@@ -142,11 +141,12 @@
 src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
 src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
 src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
 src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
 src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
 src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
 src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
+src/alpaca_eval/models_configs/wizardlm-13b-v1.2/configs.yaml
 tests/test_analyze.py
 tests/test_decoders_unit.py
 tests/test_main.py
 tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.2.6/src/alpaca_eval.egg-info/requires.txt` & `alpaca_eval-0.2.7/src/alpaca_eval.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/tests/test_analyze.py` & `alpaca_eval-0.2.7/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/tests/test_decoders_unit.py` & `alpaca_eval-0.2.7/tests/test_decoders_unit.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/tests/test_main.py` & `alpaca_eval-0.2.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.6/tests/test_pairwise_evaluator.py` & `alpaca_eval-0.2.7/tests/test_pairwise_evaluator.py`

 * *Files identical despite different names*


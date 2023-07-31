# Comparing `tmp/keras-nlp-0.6.0.dev0.tar.gz` & `tmp/keras-nlp-0.6.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-nlp-0.6.0.dev0.tar", last modified: Mon Jul 10 23:46:06 2023, max compression
+gzip compressed data, was "keras-nlp-0.6.1.dev0.tar", last modified: Mon Jul 31 21:38:05 2023, max compression
```

## Comparing `keras-nlp-0.6.0.dev0.tar` & `keras-nlp-0.6.1.dev0.tar`

### file list

```diff
@@ -1,334 +1,336 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.196850 keras-nlp-0.6.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-10 23:46:06.196850 keras-nlp-0.6.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.160850 keras-nlp-0.6.0.dev0/keras_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-10 23:46:00.000000 keras-nlp-0.6.0.dev0/keras_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.160850 keras-nlp-0.6.0.dev0/keras_nlp/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-10 23:46:00.000000 keras-nlp-0.6.0.dev0/keras_nlp/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.160850 keras-nlp-0.6.0.dev0/keras_nlp/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-10 23:46:00.000000 keras-nlp-0.6.0.dev0/keras_nlp/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.160850 keras-nlp-0.6.0.dev0/keras_nlp/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-10 23:46:00.000000 keras-nlp-0.6.0.dev0/keras_nlp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.160850 keras-nlp-0.6.0.dev0/keras_nlp/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-10 23:46:00.000000 keras-nlp-0.6.0.dev0/keras_nlp/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.160850 keras-nlp-0.6.0.dev0/keras_nlp/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.160850 keras-nlp-0.6.0.dev0/keras_nlp/src/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/backend/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/backend/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/backend/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.160850 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.164850 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/f_net_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/f_net_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/masked_lm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/masked_lm_head_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/sine_position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/sine_position_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20778 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_decoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.164850 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/preprocessing_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/random_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/random_deletion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/random_swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/random_swap_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/start_end_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/start_end_packer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.168850 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/bleu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/edit_distance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/perplexity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/rouge_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/rouge_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/rouge_l_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/rouge_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/rouge_n_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.168850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.168850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.172850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21683 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.172850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.176850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/relative_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.176850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.180850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/generative_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.180850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.180850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/rotary_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.184850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_causal_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.184850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.184850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_transformer_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/task_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.188850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18308 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.188850 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.192850 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/beam_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/beam_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/contrastive_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/contrastive_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/greedy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/greedy_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/random_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/top_k_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/top_k_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/top_p_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/top_p_sampler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.192850 keras-nlp-0.6.0.dev0/keras_nlp/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.192850 keras-nlp-0.6.0.dev0/keras_nlp/src/tests/doc_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tests/doc_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tests/doc_tests/docstring_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tests/doc_tests/docstring_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tests/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.192850 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24895 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/byte_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/byte_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.196850 keras-nlp-0.6.0.dev0/keras_nlp/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/utils/keras_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/utils/keras_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/utils/pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/utils/pipeline_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/utils/python_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/utils/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/keras_nlp/src/utils/tensor_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.196850 keras-nlp-0.6.0.dev0/keras_nlp/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-10 23:46:00.000000 keras-nlp-0.6.0.dev0/keras_nlp/tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:46:06.160850 keras-nlp-0.6.0.dev0/keras_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-10 23:46:06.000000 keras-nlp-0.6.0.dev0/keras_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-07-10 23:46:06.000000 keras-nlp-0.6.0.dev0/keras_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 23:46:06.000000 keras-nlp-0.6.0.dev0/keras_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-10 23:46:06.000000 keras-nlp-0.6.0.dev0/keras_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:46:06.000000 keras-nlp-0.6.0.dev0/keras_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-10 23:46:06.196850 keras-nlp-0.6.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-10 23:45:53.000000 keras-nlp-0.6.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.827526 keras-nlp-0.6.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-31 21:38:05.827526 keras-nlp-0.6.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.791525 keras-nlp-0.6.1.dev0/keras_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-31 21:37:59.000000 keras-nlp-0.6.1.dev0/keras_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.791525 keras-nlp-0.6.1.dev0/keras_nlp/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-31 21:37:59.000000 keras-nlp-0.6.1.dev0/keras_nlp/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.791525 keras-nlp-0.6.1.dev0/keras_nlp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 21:37:59.000000 keras-nlp-0.6.1.dev0/keras_nlp/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.791525 keras-nlp-0.6.1.dev0/keras_nlp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-31 21:37:59.000000 keras-nlp-0.6.1.dev0/keras_nlp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.791525 keras-nlp-0.6.1.dev0/keras_nlp/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-31 21:37:59.000000 keras-nlp-0.6.1.dev0/keras_nlp/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.791525 keras-nlp-0.6.1.dev0/keras_nlp/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.791525 keras-nlp-0.6.1.dev0/keras_nlp/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/backend/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/backend/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/backend/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.791525 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.795525 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/f_net_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/f_net_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/masked_lm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/masked_lm_head_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/sine_position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/sine_position_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20778 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.795525 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/preprocessing_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/random_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/random_deletion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/random_swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/random_swap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/start_end_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/start_end_packer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.795525 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/bleu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/edit_distance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/perplexity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/rouge_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/rouge_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/rouge_l_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/rouge_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/rouge_n_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.799525 keras-nlp-0.6.1.dev0/keras_nlp/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.799525 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.803525 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21737 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.803525 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.807525 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/relative_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.807525 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.807525 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/generative_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.811525 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.811525 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/rotary_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.815526 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.815526 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.815526 keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_transformer_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/task_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.819526 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18308 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.819526 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.823526 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/beam_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/beam_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/contrastive_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/contrastive_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/greedy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/greedy_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/random_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/top_k_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/top_k_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/top_p_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/top_p_sampler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.823526 keras-nlp-0.6.1.dev0/keras_nlp/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.823526 keras-nlp-0.6.1.dev0/keras_nlp/src/tests/doc_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tests/doc_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tests/doc_tests/docstring_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tests/doc_tests/docstring_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tests/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.823526 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24895 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/byte_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/byte_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.827526 keras-nlp-0.6.1.dev0/keras_nlp/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/utils/keras_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/utils/keras_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/utils/pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/utils/pipeline_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/utils/python_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/utils/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/keras_nlp/src/utils/tensor_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.827526 keras-nlp-0.6.1.dev0/keras_nlp/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-31 21:37:59.000000 keras-nlp-0.6.1.dev0/keras_nlp/tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:38:05.791525 keras-nlp-0.6.1.dev0/keras_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-31 21:38:05.000000 keras-nlp-0.6.1.dev0/keras_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-07-31 21:38:05.000000 keras-nlp-0.6.1.dev0/keras_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:38:05.000000 keras-nlp-0.6.1.dev0/keras_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 21:38:05.000000 keras-nlp-0.6.1.dev0/keras_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 21:38:05.000000 keras-nlp-0.6.1.dev0/keras_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-31 21:38:05.827526 keras-nlp-0.6.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-31 21:37:56.000000 keras-nlp-0.6.1.dev0/setup.py
```

### Comparing `keras-nlp-0.6.0.dev0/PKG-INFO` & `keras-nlp-0.6.1.dev0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,23 @@
-Metadata-Version: 2.1
-Name: keras-nlp
-Version: 0.6.0.dev0
-Summary: Industry-strength Natural Language Processing extensions for Keras.
-Home-page: https://github.com/keras-team/keras-nlp
-Author: Keras team
-Author-email: keras-nlp@google.com
-License: Apache License 2.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: extras
-
 # KerasNLP: Modular NLP Workflows for Keras
 [![](https://github.com/keras-team/keras-nlp/workflows/Tests/badge.svg?branch=master)](https://github.com/keras-team/keras-nlp/actions?query=workflow%3ATests+branch%3Amaster)
 ![Python](https://img.shields.io/badge/python-v3.8.0+-success.svg)
 ![Tensorflow](https://img.shields.io/badge/tensorflow-v2.5.0+-success.svg)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/keras-team/keras-nlp/issues)
 
-
-KerasNLP is a natural language processing library that supports users through
-their entire development cycle. Our workflows are built from modular components 
-that have state-of-the-art preset weights and architectures when used 
-out-of-the-box and are easily customizable when more control is needed. We 
-emphasize in-graph computation for all workflows so that developers can expect 
-easy productionization using the TensorFlow ecosystem.
+KerasNLP is a natural language processing library that works natively 
+with TensorFlow, JAX, or PyTorch. Built on [Keras Core](https://keras.io/keras_core/announcement/),
+these models, layers, metrics, callbacks, etc., can be trained and serialized
+in any framework and re-used in another without costly migrations. See "Using 
+KerasNLP with Keras Core" below for more details on multi-framework KerasNLP.
+
+KerasNLP supports users through their entire development cycle. Our workflows 
+are built from modular components that have state-of-the-art preset weights and 
+architectures when used out-of-the-box and are easily customizable when more 
+control is needed.
 
 This library is an extension of the core Keras API; all high-level modules are 
 [`Layers`](https://keras.io/api/layers/) or 
 [`Models`](https://keras.io/api/models/) that receive that same level of polish 
 as core Keras. If you are familiar with Keras, congratulations! You already 
 understand most of KerasNLP.
 
@@ -77,14 +55,42 @@
 
 To install the latest unreleased changes to the library, we recommend using
 pip to install directly from the master branch on github:
 
 ```
 pip install git+https://github.com/keras-team/keras-nlp.git --upgrade
 ```
+## Using KerasNLP with Keras Core
+
+As of version `0.6.0`, KerasNLP supports multiple backends with Keras Core out 
+of the box. There are two ways to configure KerasNLP to run with multi-backend 
+support:
+
+1. Via the `KERAS_BACKEND` environment variable. If set, then KerasNLP will be 
+using Keras Core with the backend specified (e.g., `KERAS_BACKEND=jax`).
+2. Via the `.keras/keras.json` and `.keras/keras_nlp.json` config files (which 
+are automatically created the first time you import KerasNLP):
+   - Set your backend of choice in `.keras/keras.json`; e.g., `"backend": "jax"`. 
+   - Set `"multi_backend": True` in `.keras/keras_nlp.json`.
+
+Once that configuration step is done, you can just import KerasNLP and start 
+using it on top of your backend of choice:
+
+```python
+import keras_nlp
+
+gpt2_lm = keras_nlp.models.GPT2CausalLM.from_preset("gpt2_base_en")
+gpt2_lm.generate("My trip to Yosemite was", max_length=200)
+```
+
+Until Keras Core is officially released as Keras 3.0, KerasNLP will use 
+`tf.keras` as the default backend. To restore this default behavior, simply 
+`unset KERAS_BACKEND` and ensure that  `"multi_backend": False` or is unset in 
+`.keras/keras_nlp.json`. You will need to restart the Python runtime for changes 
+to take effect.
 
 ## Quickstart
 
 Fine-tune BERT on a small sentiment analysis task using the 
 [`keras_nlp.models`](https://keras.io/api/keras_nlp/models/) API:
 
 ```python
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/layers/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/models/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 from keras_nlp.src.models.gpt2.gpt2_backbone import GPT2Backbone
 from keras_nlp.src.models.gpt2.gpt2_causal_lm import GPT2CausalLM
 from keras_nlp.src.models.gpt2.gpt2_causal_lm_preprocessor import GPT2CausalLMPreprocessor
 from keras_nlp.src.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
 from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_causal_lm import GPTNeoXCausalLM
 from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
 from keras_nlp.src.models.opt.opt_causal_lm import OPTCausalLM
 from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import OPTCausalLMPreprocessor
 from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
 from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
 from keras_nlp.src.models.roberta.roberta_classifier import RobertaClassifier
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/samplers/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 from keras_nlp.src import metrics
 from keras_nlp.src import models
 from keras_nlp.src import samplers
 from keras_nlp.src import tokenizers
 from keras_nlp.src import utils
 
 # This is the global source of truth for the version number.
-__version__ = "0.6.0.dev0"
+__version__ = "0.6.1.dev0"
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/api_export.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/backend/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/backend/config.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/backend/keras.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/backend/keras.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/backend/ops.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/backend/ops.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/backend/random.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/backend/random.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/conftest.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/conftest.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/f_net_encoder.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/f_net_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """FNet encoder block implementation based on `keras.layers.Layer`."""
 
-import tensorflow as tf
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
+from keras_nlp.src.backend import ops
 from keras_nlp.src.utils.keras_utils import clone_initializer
-from keras_nlp.src.utils.tensor_utils import assert_tf_backend
 
 
 @keras_nlp_export("keras_nlp.layers.FNetEncoder")
 class FNetEncoder(keras.layers.Layer):
     """FNet encoder.
 
     This class follows the architecture of FNet encoder layer in the
@@ -58,20 +57,20 @@
 
     ```python
     # Create a single FNet encoder layer.
     encoder = keras_nlp.layers.FNetEncoder(
         intermediate_dim=64)
 
     # Create a simple model containing the encoder.
-    input = keras.Input(shape=[10, 64])
+    input = keras.Input(shape=(10, 64))
     output = encoder(input)
     model = keras.Model(inputs=input, outputs=output)
 
     # Call encoder on the inputs.
-    input_data = tf.random.uniform(shape=[1, 10, 64])
+    input_data = np.random.uniform(size=(1, 10, 64))
     output = model(input_data)
     ```
 
     References:
      - [Lee-Thorp et al., 2021](https://arxiv.org/abs/2105.03824)
     """
 
@@ -82,16 +81,14 @@
         activation="relu",
         layer_norm_epsilon=1e-5,
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         name=None,
         **kwargs
     ):
-        assert_tf_backend(self.__class__.__name__)
-
         super().__init__(name=name, **kwargs)
         self.intermediate_dim = intermediate_dim
         self.dropout = dropout
         self.activation = keras.activations.get(activation)
         self.layer_norm_epsilon = layer_norm_epsilon
         self.kernel_initializer = keras.initializers.get(kernel_initializer)
         self.bias_initializer = keras.initializers.get(bias_initializer)
@@ -137,19 +134,17 @@
 
         Returns:
             A Tensor of the same shape as the `inputs`.
         """
 
         def fourier_transform(input):
             # Apply FFT on the input and take the real part.
-            # Before we apply fourier transform, let's convert the dtype of the
-            # input tensor to complex64.
-            x = tf.cast(input, tf.complex64)
-            mixing_output = tf.math.real(tf.signal.fft2d(x))
-            return tf.cast(mixing_output, input.dtype)
+            real_in, imaginary_in = (input, ops.zeros_like(input))
+            real_out, _ = ops.fft2((real_in, imaginary_in))
+            return real_out
 
         def add_and_norm(input1, input2, norm_layer):
             return norm_layer(input1 + input2)
 
         def feed_forward(input):
             x = self._intermediate_dense(input)
             x = self._output_dense(x)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/f_net_encoder_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/f_net_encoder_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for FNet Encoder."""
 
 import os
 
-import pytest
-
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling import f_net_encoder
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
 class FNetEncoderTest(TestCase):
     def test_valid_call(self):
         encoder = f_net_encoder.FNetEncoder(intermediate_dim=4)
         model = keras.Sequential(
             [
                 keras.Input(shape=(4, 6)),
                 encoder,
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/masked_lm_head.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/masked_lm_head.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,15 +119,14 @@
         self.intermediate_activation = keras.activations.get(
             intermediate_activation
         )
         self.activation = keras.activations.get(activation)
         self.layer_norm_epsilon = layer_norm_epsilon
         self.kernel_initializer = keras.initializers.get(kernel_initializer)
         self.bias_initializer = keras.initializers.get(bias_initializer)
-        self._built = False
 
         if vocabulary_size is None and embedding_weights is None:
             raise ValueError(
                 "One of `vocabulary_size` or `embedding_weights` must be set. "
                 "Received: `vocabulary_size=None`, `embedding_weights=None`"
             )
 
@@ -138,53 +137,54 @@
                     "`vocabulary_size` should match the first dimension of the "
                     "shape of `embedding_weights`. Received: "
                     f"`vocabulary_size={vocabulary_size}`, "
                     f"`embedding_weights.shape={shape}`"
                 )
             self.vocabulary_size = shape[0]
 
-    def build(self, inputs_shape, masked_positions_shape=None):
+    def build(self, inputs_shape):
         if self.embedding_weights is not None:
             feature_size = self.embedding_weights.shape[-1]
         else:
             feature_size = inputs_shape[-1]
 
         self._dense = keras.layers.Dense(
             feature_size,
             activation=self.intermediate_activation,
             kernel_initializer=self.kernel_initializer,
             bias_initializer=self.bias_initializer,
         )
         self._layer_norm = keras.layers.LayerNormalization(
             epsilon=self.layer_norm_epsilon,
         )
-        if masked_positions_shape:
-            gather_length = masked_positions_shape[1]
-            shape = (inputs_shape[0], gather_length, inputs_shape[-1])
-            self._dense.build(shape)
-            shape = (inputs_shape[0], gather_length, feature_size)
-            self._layer_norm.build(shape)
+        # The gather length does not affect any of our built variables, so
+        # we can pass any value here.
+        gather_length = None
+        shape = (inputs_shape[0], gather_length, inputs_shape[-1])
+        self._dense.build(shape)
+        shape = (inputs_shape[0], gather_length, feature_size)
+        self._layer_norm.build(shape)
         if self.embedding_weights is None:
             self._kernel = self.add_weight(
                 name="output_kernel",
                 shape=[feature_size, self.vocabulary_size],
                 initializer=self.kernel_initializer,
                 dtype=self.dtype,
             )
         self._bias = self.add_weight(
             name="output_bias",
             shape=[self.vocabulary_size],
             initializer=self.bias_initializer,
             dtype=self.dtype,
         )
 
-    def call(self, inputs, masked_positions):
+    def call(self, inputs, mask_positions):
         # Gather the encoded tokens at the masked indices.
-        masked_positions = ops.expand_dims(masked_positions, axis=-1)
-        x = ops.take_along_axis(inputs, masked_positions, axis=1)
+        mask_positions = ops.expand_dims(mask_positions, axis=-1)
+        x = ops.take_along_axis(inputs, mask_positions, axis=1)
 
         # Apply a trainable linear transformation and a layer norm.
         x = self._dense(x)
         x = self._layer_norm(x)
 
         # Transform encodings to vocabulary_size predictions.
         if self.embedding_weights is None:
@@ -217,12 +217,14 @@
                 "bias_initializer": keras.initializers.serialize(
                     self.bias_initializer
                 ),
             }
         )
         return config
 
-    def compute_output_shape(self, inputs_shape, masked_positions_shape):
-        output_shape = list(masked_positions_shape)
-        output_shape[-1] = self.vocabulary_size
-        return tuple(output_shape)
+    # TODO: restore this after https://github.com/keras-team/keras-core/pull/632
+    # is in a release!
+    # def compute_output_shape(self, inputs_shape, mask_positions_shape):
+    #     output_shape = list(mask_positions_shape)
+    #     output_shape[-1] = self.vocabulary_size
+    #     return tuple(output_shape)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/masked_lm_head_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/masked_lm_head_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def test_valid_call(self):
         head = masked_lm_head.MaskedLMHead(
             vocabulary_size=100,
             activation="softmax",
         )
         encoded_tokens = keras.Input(shape=(10, 16))
         positions = keras.Input(shape=(5,), dtype="int32")
-        outputs = head(encoded_tokens, masked_positions=positions)
+        outputs = head(encoded_tokens, mask_positions=positions)
         model = keras.Model((encoded_tokens, positions), outputs)
 
         token_data = ops.random.uniform(shape=(4, 10, 16))
         position_data = ops.random.randint(minval=0, maxval=10, shape=(4, 5))
         model((token_data, position_data))
 
     def test_valid_call_with_embedding_weights(self):
@@ -44,15 +44,15 @@
             embedding_weights=embedding.embeddings,
             activation="softmax",
         )
         # Use a difference "hidden dim" for the model than "embedding dim", we
         # need to support this in the layer.
         sequence = keras.Input(shape=(10, 32))
         positions = keras.Input(shape=(5,), dtype="int32")
-        outputs = head(sequence, masked_positions=positions)
+        outputs = head(sequence, mask_positions=positions)
         model = keras.Model((sequence, positions), outputs)
         sequence_data = ops.random.uniform(shape=(4, 10, 32))
         position_data = ops.random.randint(minval=0, maxval=10, shape=(4, 5))
         model((sequence_data, position_data))
 
     def test_get_config_and_from_config(self):
         head = masked_lm_head.MaskedLMHead(
@@ -102,15 +102,15 @@
 
     def test_one_train_step(self):
         head = masked_lm_head.MaskedLMHead(
             vocabulary_size=100,
         )
         encoded_tokens = keras.Input(shape=(10, 16))
         positions = keras.Input(shape=(5,), dtype="int32")
-        outputs = head(encoded_tokens, masked_positions=positions)
+        outputs = head(encoded_tokens, mask_positions=positions)
         model = keras.Model((encoded_tokens, positions), outputs)
 
         token_data = ops.random.uniform(shape=(4, 10, 16))
         position_data = ops.random.randint(minval=0, maxval=10, shape=(4, 5))
         label_data = ops.random.randint(minval=0, maxval=2, shape=(4, 5, 1))
 
         loss = keras.losses.SparseCategoricalCrossentropy(from_logits=False)
@@ -122,15 +122,15 @@
     def test_saved_model(self):
         head = masked_lm_head.MaskedLMHead(
             vocabulary_size=100,
             activation="softmax",
         )
         encoded_tokens = keras.Input(shape=(10, 16))
         positions = keras.Input(shape=(5,), dtype="int32")
-        outputs = head(encoded_tokens, masked_positions=positions)
+        outputs = head(encoded_tokens, mask_positions=positions)
         model = keras.Model((encoded_tokens, positions), outputs)
 
         token_data = ops.random.uniform(shape=(4, 10, 16))
         position_data = ops.random.randint(minval=0, maxval=10, shape=(4, 5))
         model_output = model((token_data, position_data))
         path = os.path.join(self.get_temp_dir(), "model.keras")
         model.save(path, save_format="keras_v3")
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/position_embedding.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/position_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/position_embedding_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/position_embedding_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for position embedding layer."""
 
 import os
 
+import numpy as np
+
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling import position_embedding
 from keras_nlp.src.tests.test_case import TestCase
 
 
 def custom_init(shape, dtype=None):
@@ -135,15 +137,15 @@
         # should trigger a down-slice.
         input_length = 17
         # Note: This test explicitly uses a batch size of 1. This is to get
         # around Keras' restriction on Model invocations: inputs are expected to
         # have the same batch cardinality as outputs. In practice, this layer
         # should be used inside a model, where it can be projected when added to
         # another tensor.
-        input_data = ops.ones(shape=[1, input_length, feature_size])
+        input_data = np.ones(shape=[1, input_length, feature_size])
         output_data = model.predict(input_data)
 
         self.assertAllEqual([1, input_length, feature_size], output_data.shape)
 
     def test_callable_initializer(self):
         max_sequence_length = 4
         feature_size = 3
@@ -152,20 +154,20 @@
             initializer=custom_init,
         )
         inputs = keras.Input(shape=(max_sequence_length, feature_size))
         outputs = test_layer(inputs)
         model = keras.Model(inputs=inputs, outputs=outputs)
 
         batch_size = 2
-        data = ops.zeros(shape=[batch_size, max_sequence_length, feature_size])
+        data = np.zeros(shape=[batch_size, max_sequence_length, feature_size])
         model(data)
         model_output = model.predict(data)
-        expected_output = ops.broadcast_to(
-            ops.reshape(
-                ops.arange(max_sequence_length * feature_size),
+        expected_output = np.broadcast_to(
+            np.reshape(
+                np.arange(max_sequence_length * feature_size),
                 [max_sequence_length, feature_size],
             ),
             [batch_size, max_sequence_length, feature_size],
         )
         self.assertAllClose(model_output, expected_output)
 
     def test_one_training_step(self):
@@ -208,15 +210,15 @@
         test_layer = position_embedding.PositionEmbedding(
             sequence_length=max_sequence_length
         )
         inputs = keras.Input(shape=(max_sequence_length, feature_size))
         outputs = test_layer(inputs)
         model = keras.Model(inputs=inputs, outputs=outputs)
 
-        data = ops.zeros(shape=[2, max_sequence_length, feature_size])
+        data = np.zeros(shape=[2, max_sequence_length, feature_size])
         model(data)
 
         path = os.path.join(self.get_temp_dir(), "model.keras")
         model.save(path, save_format="keras_v3")
         loaded_model = keras.models.load_model(path)
 
         model_output = model.predict(data)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/sine_position_encoding.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/sine_position_encoding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/sine_position_encoding_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/sine_position_encoding_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for TokenAndPositionEmbedding"""
 
 import os
 
+import numpy as np
+
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling.token_and_position_embedding import (
     TokenAndPositionEmbedding,
 )
 from keras_nlp.src.tests.test_case import TestCase
 
 
 class TokenAndPositionEmbeddingTest(TestCase):
@@ -63,27 +64,27 @@
         )
         # Create a 2-dimensional input
         # (the first dimension is implicit).
         inputs = keras.Input(shape=(sequence_length,), dtype="int32")
         outputs = test_layer(inputs)
         model = keras.Model(inputs, outputs)
 
-        input_data = ops.ones((2, sequence_length), dtype="int32")
-        expected_output_data = ops.ones((2, sequence_length, embedding_dim)) * 2
+        input_data = np.ones((2, sequence_length), dtype="int32")
+        expected_output_data = np.ones((2, sequence_length, embedding_dim)) * 2
         output_data = model.predict(input_data)
         self.assertAllClose(output_data, expected_output_data)
 
     def test_mask_propagation(self):
         test_layer = TokenAndPositionEmbedding(
             vocabulary_size=5,
             sequence_length=4,
             embedding_dim=3,
             mask_zero=True,
         )
-        input_data = ops.array([[1, 0], [1, 0]])
+        input_data = np.array([[1, 0], [1, 0]])
         mask = input_data != 0
         outputs = test_layer(input_data)
         self.assertAllEqual(outputs._keras_mask, mask)
 
     def test_saved_model(self):
         vocabulary_size = 5
         sequence_length = 4
@@ -93,15 +94,15 @@
             sequence_length=sequence_length,
             embedding_dim=embedding_dim,
         )
         inputs = keras.Input(shape=(sequence_length,))
         outputs = test_layer(inputs)
         model = keras.Model(inputs=inputs, outputs=outputs)
 
-        data = ops.zeros(shape=[2, sequence_length])
+        data = np.zeros(shape=[2, sequence_length])
         model(data)
 
         path = os.path.join(self.get_temp_dir(), "model.keras")
         model.save(path, save_format="keras_v3")
         loaded_model = keras.models.load_model(path)
 
         model_output = model.predict(data)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_decoder.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_decoder_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_decoder_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_encoder.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_encoder_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_encoder_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import numpy as np
 import tensorflow as tf
 
+from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.preprocessing.masked_lm_mask_generator import (
     MaskedLMMaskGenerator,
 )
 from keras_nlp.src.tests.test_case import TestCase
 
 
 class MaskedLMMaskGeneratorTest(TestCase):
@@ -139,15 +139,15 @@
             mask_selection_length=5,
             unselectable_token_ids=unselectable_token_ids,
             mask_token_rate=1,
             random_token_rate=0,
         )
         outputs = masked_lm_masker([unselectable_token_ids])
         # Verify that no token is masked out.
-        self.assertEqual(np.sum(np.array(outputs["mask_weights"])), 0)
+        self.assertEqual(ops.sum(outputs["mask_weights"]), 0)
 
     def test_config(self):
         unselectable_token_ids = [
             self.vocabulary_size - 1,
             self.vocabulary_size - 2,
         ]
         masked_lm_masker = MaskedLMMaskGenerator(
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/preprocessing_layer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/preprocessing_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/random_deletion.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/random_deletion.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/random_deletion_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/random_deletion_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/random_swap.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/random_swap.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/random_swap_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/random_swap_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/start_end_packer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/start_end_packer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/layers/preprocessing/start_end_packer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/layers/preprocessing/start_end_packer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/bleu.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/bleu.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import collections
 import math
 
 import tensorflow as tf
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
-from keras_nlp.src.utils.tensor_utils import assert_tf_backend
+from keras_nlp.src.backend import ops
 from keras_nlp.src.utils.tensor_utils import is_floating_dtype
 from keras_nlp.src.utils.tensor_utils import tensor_to_list
 
 REPLACE_SUBSTRINGS = [
     ("<skipped>", ""),
     ("-\n", ""),
     ("\n", " "),
@@ -108,16 +108,14 @@
         tokenizer=None,
         max_order=4,
         smooth=False,
         dtype="float32",
         name="bleu",
         **kwargs,
     ):
-        assert_tf_backend(self.__class__.__name__)
-
         super().__init__(name=name, dtype=dtype, **kwargs)
 
         if not is_floating_dtype(dtype):
             raise ValueError(
                 "`dtype` must be a floating point type. "
                 f"Received: dtype={dtype}"
             )
@@ -286,16 +284,18 @@
             matches_by_order,
             possible_matches_by_order,
             translation_length,
             reference_length,
         )
 
     def _calculate_bleu_score(self, references, translation):
-        references = tensor_to_list(references)
-        translation = tensor_to_list(translation)
+        if isinstance(references, (tf.Tensor, tf.RaggedTensor)):
+            references = tensor_to_list(references)
+        if isinstance(translation, (tf.Tensor, tf.RaggedTensor)):
+            translation = tensor_to_list(translation)
 
         matches = self._matches.numpy()
         possible_matches = self._possible_matches.numpy()
         translation_length = self._translation_length.numpy()
         reference_length = self._reference_length.numpy()
 
         (
@@ -311,19 +311,19 @@
             possible_matches_by_order=possible_matches,
             translation_length=translation_length,
             reference_length=reference_length,
             max_order=self.max_order,
             smooth=self.smooth,
         )
         return (
-            tf.constant(bleu_score, dtype=self.dtype),
-            tf.constant(matches, dtype=self.dtype),
-            tf.constant(possible_matches, dtype=self.dtype),
-            tf.constant(translation_length, dtype=self.dtype),
-            tf.constant(reference_length, dtype=self.dtype),
+            bleu_score,
+            matches,
+            possible_matches,
+            translation_length,
+            reference_length,
         )
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         def validate_and_fix_rank(inputs, tensor_name, base_rank=0):
             if not isinstance(inputs, (tf.Tensor, tf.RaggedTensor)):
                 inputs = tf.convert_to_tensor(inputs)
 
@@ -353,35 +353,31 @@
 
         (
             bleu_score,
             matches,
             possible_matches,
             translation_length,
             reference_length,
-        ) = tf.py_function(
-            func=self._calculate_bleu_score,
-            inp=[y_true, y_pred],
-            Tout=[self.dtype, self.dtype, self.dtype, self.dtype, self.dtype],
-        )
+        ) = self._calculate_bleu_score(y_true, y_pred)
 
         self._matches.assign(matches)
         self._possible_matches.assign(possible_matches)
         self._translation_length.assign(translation_length)
         self._reference_length.assign(reference_length)
         self._bleu.assign(bleu_score)
 
     def result(self):
         return self._bleu
 
     def reset_state(self):
         self._matches.assign(
-            tf.zeros(shape=(self.max_order,), dtype=self.dtype)
+            ops.zeros(shape=(self.max_order,), dtype=self.dtype)
         )
         self._possible_matches.assign(
-            tf.zeros(shape=(self.max_order,), dtype=self.dtype)
+            ops.zeros(shape=(self.max_order,), dtype=self.dtype)
         )
         self._translation_length.assign(0.0)
         self._reference_length.assign(0.0)
         self._bleu.assign(0.0)
 
     def get_config(self):
         config = super().get_config()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/bleu_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/bleu_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.metrics.bleu import Bleu
 from keras_nlp.src.tests.test_case import TestCase
 from keras_nlp.src.tokenizers.byte_tokenizer import ByteTokenizer
 
 
-@pytest.mark.tf_only
 class BleuTest(TestCase):
     def test_initialization(self):
         bleu = Bleu()
         result = bleu.result()
 
         self.assertEqual(result, 0.0)
 
@@ -65,87 +64,62 @@
             ["He He He eats sweet apple which is a fruit."],
             ["I love Silicon Valley, it's one of my favourite shows."],
         ]
 
         bleu_val = bleu(y_true, y_pred)
         self.assertAlmostEqual(bleu_val, 0.243, delta=1e-3)
 
-    def test_1d_tensor_input(self):
-        bleu = Bleu()
-        y_true = tf.ragged.constant(
-            [
-                ["He eats a sweet apple."],
-                ["Silicon Valley is one of my favourite shows!"],
-            ]
-        )
-        y_pred = tf.constant(
-            [
-                "He He He eats sweet apple which is a fruit.",
-                "I love Silicon Valley, it's one of my favourite shows.",
-            ]
-        )
-
-        bleu_val = bleu(y_true, y_pred)
-        self.assertAlmostEqual(bleu_val, 0.243, delta=1e-3)
-
-    def test_2d_tensor_input(self):
-        bleu = Bleu()
-        y_true = tf.constant(
-            [
-                [["He eats a sweet apple."]],
-                [["Silicon Valley is one of my favourite shows!"]],
-            ]
-        )
-        y_pred = tf.constant(
-            [
-                ["He He He eats sweet apple which is a fruit."],
-                ["I love Silicon Valley, it's one of my favourite shows."],
-            ]
-        )
-
-        bleu_val = bleu(y_true, y_pred)
-        self.assertAlmostEqual(bleu_val, 0.243, delta=1e-3)
-
     def test_custom_tokenizer(self):
         byte_tokenizer = ByteTokenizer()
         bleu = Bleu(tokenizer=byte_tokenizer)
-        y_true = tf.ragged.constant(
-            [
-                ["He eats a sweet apple."],
-                ["Silicon Valley is one of my favourite shows!"],
-            ]
-        )
-        y_pred = tf.constant(
-            [
-                "He He He eats sweet apple which is a fruit.",
-                "I love Silicon Valley, it's one of my favourite shows.",
-            ]
-        )
+        y_true = [
+            ["He eats a sweet apple."],
+            ["Silicon Valley is one of my favourite shows!"],
+        ]
+        y_pred = [
+            "He He He eats sweet apple which is a fruit.",
+            "I love Silicon Valley, it's one of my favourite shows.",
+        ]
 
         bleu_val = bleu(y_true, y_pred)
         self.assertAlmostEqual(bleu_val, 0.609, delta=1e-3)
 
     def test_different_order(self):
         bleu = Bleu(max_order=5)
-        y_true = tf.ragged.constant(
+        y_true = [
+            ["He eats a sweet apple."],
+            ["Silicon Valley is one of my favourite shows!"],
+        ]
+        y_pred = [
+            "He He He eats sweet apple which is a fruit.",
+            "I love Silicon Valley, it's one of my favourite shows.",
+        ]
+
+        bleu_val = bleu(y_true, y_pred)
+        self.assertAlmostEqual(bleu_val, 0.188, delta=1e-3)
+
+    def test_tensor_input(self):
+        bleu = Bleu()
+        y_true = tf.constant(
             [
                 ["He eats a sweet apple."],
                 ["Silicon Valley is one of my favourite shows!"],
             ]
         )
         y_pred = tf.constant(
             [
                 "He He He eats sweet apple which is a fruit.",
                 "I love Silicon Valley, it's one of my favourite shows.",
             ]
         )
 
         bleu_val = bleu(y_true, y_pred)
-        self.assertAlmostEqual(bleu_val, 0.188, delta=1e-3)
+        self.assertAlmostEqual(bleu_val, 0.243, delta=1e-3)
 
+    @pytest.mark.tf_only  # string model output only applies to tf.
     def test_model_compile(self):
         inputs = keras.Input(shape=(), dtype="string")
         outputs = keras.layers.Identity()(inputs)
         model = keras.Model(inputs, outputs)
         model.compile(metrics=[Bleu()])
 
         y_pred = x = tf.constant(
@@ -162,56 +136,48 @@
         )
 
         output = model.compute_metrics(x, y, y_pred, sample_weight=None)
         self.assertAlmostEqual(output["bleu"], 0.243, delta=1e-3)
 
     def test_reset_state(self):
         bleu = Bleu()
-        y_true = tf.ragged.constant(
-            [
-                ["He eats a sweet apple."],
-                ["Silicon Valley is one of my favourite shows!"],
-            ]
-        )
-        y_pred = tf.constant(
-            [
-                "He He He eats sweet apple which is a fruit.",
-                "I love Silicon Valley, it's one of my favourite shows.",
-            ]
-        )
+        y_true = [
+            ["He eats a sweet apple."],
+            ["Silicon Valley is one of my favourite shows!"],
+        ]
+        y_pred = [
+            "He He He eats sweet apple which is a fruit.",
+            "I love Silicon Valley, it's one of my favourite shows.",
+        ]
 
         bleu.update_state(y_true, y_pred)
         bleu_val = bleu.result()
         self.assertNotEqual(bleu_val, 0.0)
 
         bleu.reset_state()
         bleu_val = bleu.result()
         self.assertEqual(bleu_val, 0.0)
 
     def test_update_state(self):
         bleu = Bleu()
-        y_true_1 = tf.ragged.constant(
-            [
-                ["He eats a sweet apple."],
-                ["Silicon Valley is one of my favourite shows!"],
-            ]
-        )
-        y_pred_1 = tf.constant(
-            [
-                "He He He eats sweet apple which is a fruit.",
-                "I love Silicon Valley, it's one of my favourite shows.",
-            ]
-        )
+        y_true_1 = [
+            ["He eats a sweet apple."],
+            ["Silicon Valley is one of my favourite shows!"],
+        ]
+        y_pred_1 = [
+            "He He He eats sweet apple which is a fruit.",
+            "I love Silicon Valley, it's one of my favourite shows.",
+        ]
 
         bleu.update_state(y_true_1, y_pred_1)
         bleu_val = bleu.result()
         self.assertAlmostEqual(bleu_val, 0.243, delta=1e-3)
 
-        y_true_2 = tf.constant(["Virat Kohli is the GOAT."])
-        y_pred_2 = tf.constant("Virat Kohli is the greatest of all time!")
+        y_true_2 = ["Virat Kohli is the GOAT."]
+        y_pred_2 = "Virat Kohli is the greatest of all time!"
 
         bleu.update_state(y_true_2, y_pred_2)
         bleu_val = bleu.result()
         self.assertAlmostEqual(bleu_val, 0.26, delta=1e-3)
 
     def test_get_config(self):
         byte_tokenizer = ByteTokenizer()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/edit_distance.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/edit_distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 """Edit Distance metric."""
 
 import tensorflow as tf
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
-from keras_nlp.src.utils.tensor_utils import assert_tf_backend
 from keras_nlp.src.utils.tensor_utils import is_floating_dtype
 
 
 @keras_nlp_export("keras_nlp.metrics.EditDistance")
 class EditDistance(keras.metrics.Metric):
     """Edit Distance metric.
 
@@ -63,57 +62,35 @@
     Single-level Python list.
     >>> edit_distance = keras_nlp.metrics.EditDistance()
     >>> y_true = "the tiny little cat was found under the big funny bed".split()
     >>> y_pred = "the cat was found under the bed".split()
     >>> edit_distance(y_true, y_pred)
     <tf.Tensor: shape=(), dtype=float32, numpy=0.36363637>
 
-    Rank 1 tensor.
-    >>> edit_distance = keras_nlp.metrics.EditDistance()
-    >>> y_true = tf.strings.split("the tiny little cat was found under the big funny bed")
-    >>> y_pred = tf.strings.split("the cat was found under the bed")
-    >>> edit_distance(y_true, y_pred)
-    <tf.Tensor: shape=(), dtype=float32, numpy=0.36363637>
-
     Nested Python list.
     >>> edit_distance = keras_nlp.metrics.EditDistance()
     >>> y_true = [
     ...     "the tiny little cat was found under the big funny bed".split(),
     ...     "it is sunny today".split(),
     ... ]
     >>> y_pred = [
     ...     "the cat was found under the bed".split(),
     ...     "it is sunny but with a hint of cloud cover".split(),
     ... ]
     >>> edit_distance(y_true, y_pred)
     <tf.Tensor: shape=(), dtype=float32, numpy=0.73333335>
-
-    Rank 2 tensor.
-    >>> edit_distance = keras_nlp.metrics.EditDistance()
-    >>> y_true = tf.strings.split([
-    ...     "the tiny little cat was found under the big funny bed",
-    ...     "it is sunny today",
-    ... ])
-    >>> y_pred = tf.strings.split([
-    ...     "the cat was found under the bed",
-    ...     "it is sunny but with a hint of cloud cover",
-    ... ])
-    >>> edit_distance(y_true, y_pred)
-    <tf.Tensor: shape=(), dtype=float32, numpy=0.73333335>
     """
 
     def __init__(
         self,
         normalize=True,
         dtype="float32",
         name="edit_distance",
         **kwargs,
     ):
-        assert_tf_backend(self.__class__.__name__)
-
         super().__init__(name=name, dtype=dtype, **kwargs)
 
         if not is_floating_dtype(dtype):
             raise ValueError(
                 "`dtype` must be a floating point type. "
                 f"Received: dtype={dtype}"
             )
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/edit_distance_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/edit_distance_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.metrics.edit_distance import EditDistance
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
 class EditDistanceTest(TestCase):
     def test_initialization(self):
         edit_distance = EditDistance()
         result = edit_distance.result()
 
         self.assertEqual(result, 0.0)
 
@@ -47,70 +46,55 @@
             "the cat was found under the bed".split(),
             "it is sunny but with a hint of cloud cover".split(),
         ]
 
         edit_distance_val = edit_distance(y_true, y_pred)
         self.assertAlmostEqual(edit_distance_val, 0.733, delta=1e-3)
 
-    def test_rank_1_tensor_input_normalize(self):
-        edit_distance = EditDistance()
-        y_true = tf.strings.split(
-            "the tiny little cat was found under the big funny bed"
-        )
-        y_pred = tf.strings.split("the cat was found under the bed")
-
-        edit_distance_val = edit_distance(y_true, y_pred)
-        self.assertAlmostEqual(edit_distance_val, 0.364, delta=1e-3)
-
-    def test_rank_2_tensor_input_normalize(self):
-        edit_distance = EditDistance()
-        y_true = tf.strings.split(
-            [
-                "the tiny little cat was found under the big funny bed",
-                "it is sunny today",
-            ]
-        )
-        y_pred = tf.strings.split(
-            [
-                "the cat was found under the bed",
-                "it is sunny but with a hint of cloud cover",
-            ]
-        )
+    def test_1d_list_input_normalize_false(self):
+        edit_distance = EditDistance(normalize=False)
+        y_true = "the tiny little cat was found under the big funny bed".split()
+        y_pred = "the cat was found under the bed".split()
 
         edit_distance_val = edit_distance(y_true, y_pred)
-        self.assertAlmostEqual(edit_distance_val, 0.733, delta=1e-3)
+        self.assertAlmostEqual(edit_distance_val, 4.0, delta=1e-3)
 
-    def test_rank_1_tensor_input_normalize_false(self):
+    def test_2d_list_input_normalize_false(self):
         edit_distance = EditDistance(normalize=False)
-        y_true = tf.strings.split(
-            "the tiny little cat was found under the big funny bed"
-        )
-        y_pred = tf.strings.split("the cat was found under the bed")
+        y_true = [
+            "the tiny little cat was found under the big funny bed".split(),
+            "it is sunny today".split(),
+        ]
+        y_pred = [
+            "the cat was found under the bed".split(),
+            "it is sunny but with a hint of cloud cover".split(),
+        ]
 
         edit_distance_val = edit_distance(y_true, y_pred)
-        self.assertAlmostEqual(edit_distance_val, 4.0, delta=1e-3)
+        self.assertAlmostEqual(edit_distance_val, 5.5, delta=1e-3)
 
-    def test_rank_2_tensor_input_normalize_false(self):
-        edit_distance = EditDistance(normalize=False)
+    def test_tensor_input(self):
+        edit_distance = EditDistance()
         y_true = tf.strings.split(
             [
                 "the tiny little cat was found under the big funny bed",
                 "it is sunny today",
             ]
         )
         y_pred = tf.strings.split(
             [
                 "the cat was found under the bed",
                 "it is sunny but with a hint of cloud cover",
             ]
         )
 
         edit_distance_val = edit_distance(y_true, y_pred)
-        self.assertAlmostEqual(edit_distance_val, 5.5, delta=1e-3)
+        self.assertAlmostEqual(edit_distance_val, 0.733, delta=1e-3)
 
+    @pytest.mark.tf_only  # string model output only applies to tf.
     def test_model_compile_normalize(self):
         inputs = keras.Input(shape=(None,), dtype="string")
         outputs = keras.layers.Identity()(inputs)
         model = keras.Model(inputs, outputs)
 
         model.compile(metrics=[EditDistance()])
 
@@ -118,14 +102,15 @@
         y = tf.strings.split(
             ["the tiny little cat was found under the big funny bed"]
         )
 
         output = model.compute_metrics(x, y, y_pred, sample_weight=None)
         self.assertAlmostEqual(output["edit_distance"], 0.364, delta=1e-3)
 
+    @pytest.mark.tf_only  # string model output only applies to tf.
     def test_model_compile_normalize_false(self):
         inputs = keras.Input(shape=(None,), dtype="string")
         outputs = keras.layers.Identity()(inputs)
         model = keras.Model(inputs, outputs)
 
         model.compile(metrics=[EditDistance(normalize=False)])
 
@@ -133,77 +118,75 @@
         y = tf.strings.split(
             ["the tiny little cat was found under the big funny bed"]
         )
 
         output = model.compute_metrics(x, y, y_pred, sample_weight=None)
         self.assertAlmostEqual(output["edit_distance"], 4.0, delta=1e-3)
 
-    def test_reset_state_normalize(self):
+    def test_rank_1_tensor_input_normalize(self):
         edit_distance = EditDistance()
         y_true = tf.strings.split(
-            [
-                "the tiny little cat was found under the big funny bed",
-                "it is sunny today",
-            ]
-        )
-        y_pred = tf.strings.split(
-            [
-                "the cat was found under the bed",
-                "it is sunny but with a hint of cloud cover",
-            ]
+            "the tiny little cat was found under the big funny bed"
         )
+        y_pred = tf.strings.split("the cat was found under the bed")
+
+        edit_distance_val = edit_distance(y_true, y_pred)
+        self.assertAlmostEqual(edit_distance_val, 0.364, delta=1e-3)
+
+    def test_reset_state_normalize(self):
+        edit_distance = EditDistance()
+        y_true = [
+            "the tiny little cat was found under the big funny bed".split(),
+            "it is sunny today".split(),
+        ]
+        y_pred = [
+            "the cat was found under the bed".split(),
+            "it is sunny but with a hint of cloud cover".split(),
+        ]
 
         edit_distance.update_state(y_true, y_pred)
         edit_distance_val = edit_distance.result()
         self.assertNotEqual(edit_distance_val, 0.0)
 
         edit_distance.reset_state()
         edit_distance_val = edit_distance.result()
         self.assertEqual(edit_distance_val, 0.0)
 
     def test_update_state_normalize(self):
         edit_distance = EditDistance()
-        y_true_1 = tf.strings.split(
-            [
-                "the tiny little cat was found under the big funny bed",
-                "it is sunny today",
-            ]
-        )
-        y_pred_1 = tf.strings.split(
-            [
-                "the cat was found under the bed",
-                "it is sunny but with a hint of cloud cover",
-            ]
-        )
+        y_true_1 = [
+            "the tiny little cat was found under the big funny bed".split(),
+            "it is sunny today".split(),
+        ]
+        y_pred_1 = [
+            "the cat was found under the bed".split(),
+            "it is sunny but with a hint of cloud cover".split(),
+        ]
 
         edit_distance.update_state(y_true_1, y_pred_1)
         edit_distance_val = edit_distance.result()
         self.assertAlmostEqual(edit_distance_val, 0.733, delta=1e-3)
 
         y_true_2 = tf.strings.split(["what is your favourite show"])
         y_pred_2 = tf.strings.split(["my favourite show is silicon valley"])
 
         edit_distance.update_state(y_true_2, y_pred_2)
         edit_distance_val = edit_distance.result()
         self.assertAlmostEqual(edit_distance_val, 0.85, delta=1e-3)
 
     def test_update_state_normalize_false(self):
         edit_distance = EditDistance(normalize=False)
-        y_true_1 = tf.strings.split(
-            [
-                "the tiny little cat was found under the big funny bed",
-                "it is sunny today",
-            ]
-        )
-        y_pred_1 = tf.strings.split(
-            [
-                "the cat was found under the bed",
-                "it is sunny but with a hint of cloud cover",
-            ]
-        )
+        y_true_1 = [
+            "the tiny little cat was found under the big funny bed".split(),
+            "it is sunny today".split(),
+        ]
+        y_pred_1 = [
+            "the cat was found under the bed".split(),
+            "it is sunny but with a hint of cloud cover".split(),
+        ]
 
         edit_distance.update_state(y_true_1, y_pred_1)
         edit_distance_val = edit_distance.result()
         self.assertAlmostEqual(edit_distance_val, 5.5, delta=1e-3)
 
         y_true_2 = tf.strings.split(["what is your favourite show"])
         y_pred_2 = tf.strings.split(["my favourite show is silicon valley"])
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/rouge_base.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/rouge_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ROUGE metric."""
 
 
-import types
-
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.utils.tensor_utils import assert_tf_backend
+from keras_nlp.src.backend import ops
 from keras_nlp.src.utils.tensor_utils import is_floating_dtype
 from keras_nlp.src.utils.tensor_utils import tensor_to_list
 
 try:
     from rouge_score import rouge_scorer
 except ImportError:
     rouge_scorer = None
@@ -58,16 +56,14 @@
         self,
         variant="rouge2",
         use_stemmer=False,
         dtype="float32",
         name="rouge",
         **kwargs,
     ):
-        assert_tf_backend(self.__class__.__name__)
-
         super().__init__(name=name, dtype=dtype, **kwargs)
 
         if rouge_scorer is None:
             raise ImportError(
                 f"{self.__class__.__name__} requires the `rouge_score` "
                 "package. Please install it with `pip install rouge-score`."
             )
@@ -119,35 +115,14 @@
         self._number_of_samples = self.add_weight(
             shape=(),
             initializer="zeros",
             dtype=self.dtype,
             name="number_of_samples",
         )
 
-    def __new__(cls, *args, **kwargs):
-        # Temporary workaround for Keras bug with dictionary return types.
-        # Wraps `result()` with a python dictionary that also supports variable
-        # assignment. We have to do this with __new__ because the base metric
-        # class wraps the `results()` method.
-        # TODO: Remove this snippet of code once the Keras bug is fixed.
-        obj = super().__new__(cls)
-
-        class MetricDict(dict):
-            """A dictionary that supports variable assignment."""
-
-            pass
-
-        def wrap_result(result_fn):
-            return tf.__internal__.decorator.make_decorator(
-                result_fn, lambda obj, *args: MetricDict(result_fn(*args))
-            )
-
-        obj.result = types.MethodType(wrap_result(obj.result), obj)
-        return obj
-
     def update_state(self, y_true, y_pred, sample_weight=None):
         # Three possible shapes for y_true and y_pred: Python string,
         # [batch_size] and [batch_size, 1]. In the latter two cases, we have
         # strings in the tensor/list.
 
         def validate_and_fix_rank(inputs, tensor_name):
             if not isinstance(inputs, tf.Tensor):
@@ -178,31 +153,24 @@
 
         def calculate_rouge_score(reference, hypothesis):
             reference = tensor_to_list(reference)
             hypothesis = tensor_to_list(hypothesis)
             score = self._rouge_scorer.score(reference, hypothesis)[
                 self.variant
             ]
-            return tf.cast(
-                tf.constant([score.precision, score.recall, score.fmeasure]),
-                dtype=self.dtype,
-            )
+            return score.precision, score.recall, score.fmeasure
 
         for batch_idx in range(batch_size):
-            score = tf.py_function(
-                func=calculate_rouge_score,
-                inp=[y_true[batch_idx], y_pred[batch_idx]],
-                Tout=self.dtype,
-            )
+            score = calculate_rouge_score(y_true[batch_idx], y_pred[batch_idx])
             self._rouge_precision.assign_add(score[0])
             self._rouge_recall.assign_add(score[1])
             self._rouge_f1_score.assign_add(score[2])
 
         self._number_of_samples.assign_add(
-            tf.cast(batch_size, dtype=self.dtype)
+            ops.cast(batch_size, dtype=self.dtype)
         )
 
     def result(self):
         if self._number_of_samples == 0:
             return {
                 "precision": 0.0,
                 "recall": 0.0,
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/rouge_l.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/rouge_n.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,124 +8,121 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""ROUGE-L metric."""
+"""ROUGE-N metric."""
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.metrics.rouge_base import RougeBase
 
 
-@keras_nlp_export("keras_nlp.metrics.RougeL")
-class RougeL(RougeBase):
-    """ROUGE-L metric.
+@keras_nlp_export("keras_nlp.metrics.RougeN")
+class RougeN(RougeBase):
+    """ROUGE-N metric.
 
-    This class implements the ROUGE-L variant of the ROUGE metric. The ROUGE-L
+    This class implements the ROUGE-N variant of the ROUGE metric. The ROUGE-N
     metric is traditionally used for evaluating summarisation systems.
-    Succinctly put, ROUGE-L is a score based on the length of the longest
-    common subsequence present in the reference text and the hypothesis text.
+    Succinctly put, ROUGE-N is a score based on the number of matching n-grams
+    between the reference text and the hypothesis text.
 
     Note on input shapes:
     For `y_true` and `y_pred`, this class supports scalar values and batch
     inputs of shapes `()`, `(batch_size,)` and `(batch_size, 1)`.
 
     Args:
+        order: The order of n-grams which are to be matched. It should lie in
+            range [1, 9]. Defaults to `2`.
         use_stemmer: bool. Whether Porter Stemmer should be used to strip word
             suffixes to improve matching. Defaults to `False`.
         dtype: string or tf.dtypes.Dtype. Precision of metric computation. If
                not specified, it defaults to `"float32"`.
         name: string. Name of the metric instance.
         **kwargs: Other keyword arguments.
 
     References:
         - [Lin et al., 2004](https://aclanthology.org/W04-1013/)
 
     Examples:
 
-    1. Various Input Types.
-    1.1. Python string.
-    >>> rouge_l = keras_nlp.metrics.RougeL()
+    1. Python string.
+    >>> rouge_n = keras_nlp.metrics.RougeN(order=2)
     >>> y_true = "the tiny little cat was found under the big funny bed"
     >>> y_pred = "the cat was under the bed"
-    >>> rouge_l(y_true, y_pred)["f1_score"]
-    <tf.Tensor: shape=(), dtype=float32, numpy=0.7058824>
+    >>> rouge_n(y_true, y_pred)["f1_score"]
+    <tf.Tensor: shape=(), dtype=float32, numpy=0.26666668>
 
-    1.2. rank 1 inputs.
-    a. Python list.
-    >>> rouge_l = keras_nlp.metrics.RougeL()
+    2. List inputs.
+    >>> rouge_n = keras_nlp.metrics.RougeN(order=2)
     >>> y_true = [
     ...     "the tiny little cat was found under the big funny bed",
     ...     "i really love contributing to KerasNLP",
     ... ]
     >>> y_pred = [
     ...     "the cat was under the bed",
     ...     "i love contributing to KerasNLP",
     ... ]
-    >>> rouge_l(y_true, y_pred)["f1_score"]
-    <tf.Tensor: shape=(), dtype=float32, numpy=0.80748665>
+    >>> rouge_n(y_true, y_pred)["f1_score"]
+    <tf.Tensor: shape=(), dtype=float32, numpy=0.4666667>
 
-    b. Tensor
-    >>> rouge_l = keras_nlp.metrics.RougeL()
-    >>> y_true = tf.constant(
-    ...     [
-    ...         "the tiny little cat was found under the big funny bed",
-    ...         "i really love contributing to KerasNLP",
-    ...     ]
-    ... )
-    >>> y_pred = tf.constant(
-    ...     [
-    ...         "the cat was under the bed",
-    ...         "i love contributing to KerasNLP",
-    ...     ]
-    ... )
-    >>> rouge_l(y_true, y_pred)["f1_score"]
-    <tf.Tensor: shape=(), dtype=float32, numpy=0.80748665>
-
-    1.3. rank 2 inputs.
-    >>> rouge_l = keras_nlp.metrics.RougeL()
-    >>> y_true = tf.constant(
-    ...     [
-    ...         ["the tiny little cat was found under the big funny bed"],
-    ...         ["i really love contributing to KerasNLP"],
-    ...     ]
-    ... )
-    >>> y_pred = tf.constant(
-    ...     [
-    ...         ["the cat was under the bed"],
-    ...         ["i love contributing to KerasNLP"],
-    ...     ]
-    ... )
-    >>> rouge_l(y_true, y_pred)["f1_score"]
-    <tf.Tensor: shape=(), dtype=float32, numpy=0.80748665>
-
-    3. Pass the metric to `model.compile()`.
-    >>> inputs = keras.Input(shape=(), dtype='string')
-    >>> outputs = keras.layers.Identity()(inputs)
-    >>> model = keras.Model(inputs, outputs)
-    >>> model.compile(metrics=[keras_nlp.metrics.RougeL()])
-    >>> y_pred = x = tf.constant(["hello this is fun"])
-    >>> y = tf.constant(["hello this is awesome"])
-    >>> model.compute_metrics(x, y, y_pred, sample_weight=None)["f1_score"]
-    0.75
+    3. 2D inputs.
+    >>> rouge_n = keras_nlp.metrics.RougeN(order=2)
+    >>> y_true =[
+    ...     ["the tiny little cat was found under the big funny bed"],
+    ...     ["i really love contributing to KerasNLP"],
+    ... ]
+    >>> y_pred =[
+    ...     ["the cat was under the bed"],
+    ...     ["i love contributing to KerasNLP"],
+    ... ]
+    >>> rouge_n(y_true, y_pred)["f1_score"]
+    <tf.Tensor: shape=(), dtype=float32, numpy=0.4666667>
+
+    4. Trigrams.
+    >>> rouge_n = keras_nlp.metrics.RougeN(order=3)
+    >>> y_true = [
+    ...     "the tiny little cat was found under the big funny bed",
+    ...     "i really love contributing to KerasNLP",
+    ... ]
+    >>> y_pred = [
+    ...     "the cat was under the bed",
+    ...     "i love contributing to KerasNLP",
+    ... ]
+    >>> rouge_n(y_true, y_pred)["f1_score"]
+    <tf.Tensor: shape=(), dtype=float32, numpy=0.2857143>
     """
 
     def __init__(
         self,
+        order=2,
         use_stemmer=False,
-        name="rouge-l",
+        name="rouge-n",
         **kwargs,
     ):
+        if order not in range(1, 10):
+            raise ValueError(
+                "Invalid `order` value. Should lie in the range [1, 9]."
+                f"Received order={order}"
+            )
+
         super().__init__(
-            variant="rougeL",
+            variant=f"rouge{order}",
             use_stemmer=use_stemmer,
             name=name,
             **kwargs,
         )
 
+        self.order = order
+
     def get_config(self):
         config = super().get_config()
         del config["variant"]
+
+        config.update(
+            {
+                "order": self.order,
+            }
+        )
         return config
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/rouge_l_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/rouge_n_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,158 +8,175 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for RougeL."""
+"""Tests for RougeN."""
 import pytest
 import tensorflow as tf
 
-from keras_nlp.src.metrics.rouge_l import RougeL
+from keras_nlp.src.backend import keras
+from keras_nlp.src.metrics.rouge_n import RougeN
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
-class RougeLTest(TestCase):
+class RougeNTest(TestCase):
     def test_initialization(self):
-        rouge = RougeL()
+        rouge = RougeN()
         result = rouge.result()
 
-        self.assertDictEqual(
+        self.assertAllClose(
             result,
             {"precision": 0.0, "recall": 0.0, "f1_score": 0.0},
         )
 
     def test_string_input(self):
-        rouge = RougeL(use_stemmer=False)
+        rouge = RougeN(order=2, use_stemmer=False)
         y_true = "the tiny little cat was found under the big funny bed"
         y_pred = "the cat was under the bed"
 
         rouge_val = rouge(y_true, y_pred)
         self.assertAllClose(
             rouge_val,
-            {"precision": 1.0, "recall": 0.545454, "f1_score": 0.705882},
+            {"precision": 0.4, "recall": 0.2, "f1_score": 0.266666},
         )
 
     def test_string_list_input(self):
-        rouge = RougeL(use_stemmer=False)
+        rouge = RougeN(order=2, use_stemmer=False)
         y_true = [
             "the tiny little cat was found under the big funny bed",
             "i really love contributing to KerasNLP",
         ]
         y_pred = [
             "the cat was under the bed",
             "i love contributing to KerasNLP",
         ]
 
         rouge_val = rouge(y_true, y_pred)
         self.assertAllClose(
             rouge_val,
-            {"precision": 1.0, "recall": 0.689393, "f1_score": 0.807486},
+            {"precision": 0.575, "recall": 0.4, "f1_score": 0.466666},
         )
 
     def test_tensor_input(self):
-        rouge = RougeL(use_stemmer=False)
+        rouge = RougeN(order=2, use_stemmer=False)
         y_true = tf.constant(
             [
                 "the tiny little cat was found under the big funny bed",
                 "i really love contributing to KerasNLP",
             ]
         )
         y_pred = tf.constant(
             ["the cat was under the bed", "i love contributing to KerasNLP"]
         )
 
         rouge_val = rouge(y_true, y_pred)
         self.assertAllClose(
             rouge_val,
-            {"precision": 1.0, "recall": 0.689393, "f1_score": 0.807486},
+            {"precision": 0.575, "recall": 0.4, "f1_score": 0.466666},
         )
 
-    def test_rank_2_input(self):
-        rouge = RougeL(use_stemmer=False)
-        y_true = tf.constant(
-            [
-                ["the tiny little cat was found under the big funny bed"],
-                ["i really love contributing to KerasNLP"],
-            ]
-        )
-        y_pred = tf.constant(
-            [["the cat was under the bed"], ["i love contributing to KerasNLP"]]
-        )
+    @pytest.mark.tf_only  # string model output only applies to tf.
+    def test_model_compile(self):
+        inputs = keras.Input(shape=(None,), dtype="string")
+        outputs = keras.layers.Identity()(inputs)
+        model = keras.Model(inputs, outputs)
+
+        model.compile(metrics=[RougeN()])
+
+        y_pred = x = tf.constant(["hello this is fun"])
+        y = tf.constant(["hello this is awesome"])
+
+        output = model.compute_metrics(x, y, y_pred, sample_weight=None)
+        self.assertAllClose(output["precision"], 0.666666)
+        self.assertAllClose(output["recall"], 0.666666)
+        self.assertAllClose(output["f1_score"], 0.666666)
+
+    def test_incorrect_order(self):
+        with self.assertRaises(ValueError):
+            _ = RougeN(order=10)
+
+    def test_different_order(self):
+        rouge = RougeN(order=3, use_stemmer=False)
+        y_true = [
+            "the tiny little cat was found under the big funny bed",
+            "i really love contributing to KerasNLP",
+        ]
+        y_pred = [
+            "the cat was under the bed",
+            "i love contributing to KerasNLP",
+        ]
 
         rouge_val = rouge(y_true, y_pred)
         self.assertAllClose(
             rouge_val,
-            {"precision": 1.0, "recall": 0.689393, "f1_score": 0.807486},
+            {"precision": 0.333333, "recall": 0.25, "f1_score": 0.285714},
         )
 
     def test_reset_state(self):
-        rouge = RougeL()
-        y_true = tf.constant(
-            ["hey, this is great fun", "i love contributing to KerasNLP"]
-        )
-        y_pred = tf.constant(
-            [
-                "great fun indeed",
-                "KerasNLP is awesome, i love contributing to it",
-            ]
-        )
+        rouge = RougeN()
+        y_true = ["hey, this is great fun", "i love contributing to KerasNLP"]
+        y_pred = [
+            "great fun indeed",
+            "KerasNLP is awesome, i love contributing to it",
+        ]
 
         rouge.update_state(y_true, y_pred)
         rouge_val = rouge.result()
         self.assertNotAllClose(
             rouge_val,
             {"precision": 0.0, "recall": 0.0, "f1_score": 0.0},
         )
 
         rouge.reset_state()
         rouge_val = rouge.result()
-        self.assertDictEqual(
+        self.assertAllClose(
             rouge_val,
             {"precision": 0.0, "recall": 0.0, "f1_score": 0.0},
         )
 
     def test_update_state(self):
-        rouge = RougeL()
-        y_true_1 = tf.constant(
-            [
-                "the tiny little cat was found under the big funny bed",
-                "i really love contributing to KerasNLP",
-            ]
-        )
-        y_pred_1 = tf.constant(
-            ["the cat was under the bed", "i love contributing to KerasNLP"]
-        )
+        rouge = RougeN()
+        y_true_1 = [
+            "the tiny little cat was found under the big funny bed",
+            "i really love contributing to KerasNLP",
+        ]
+        y_pred_1 = [
+            "the cat was under the bed",
+            "i love contributing to KerasNLP",
+        ]
 
         rouge.update_state(y_true_1, y_pred_1)
         rouge_val = rouge.result()
         self.assertAllClose(
             rouge_val,
-            {"precision": 1.0, "recall": 0.689393, "f1_score": 0.807486},
+            {"precision": 0.575, "recall": 0.4, "f1_score": 0.466666},
         )
 
-        y_true_2 = tf.constant(["what is your favourite show"])
-        y_pred_2 = tf.constant(["my favourite show is silicon valley"])
+        y_true_2 = ["what is your favourite show"]
+        y_pred_2 = ["my favourite show is silicon valley"]
 
         rouge.update_state(y_true_2, y_pred_2)
         rouge_val = rouge.result()
         self.assertAllClose(
             rouge_val,
-            {"precision": 0.777777, "recall": 0.592929, "f1_score": 0.659536},
+            {"precision": 0.45, "recall": 0.35, "f1_score": 0.385185},
         )
 
     def test_get_config(self):
-        rouge = RougeL(
+        rouge = RougeN(
+            order=5,
             use_stemmer=True,
             dtype="float32",
-            name="rouge_l_test",
+            name="rouge_n_test",
         )
 
         config = rouge.get_config()
         expected_config_subset = {
+            "order": 5,
             "use_stemmer": True,
         }
+
         self.assertEqual(config, {**config, **expected_config_subset})
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/metrics/rouge_n_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/metrics/rouge_l_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,199 +8,133 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for RougeN."""
-import pytest
+"""Tests for RougeL."""
 import tensorflow as tf
 
-from keras_nlp.src.backend import keras
-from keras_nlp.src.metrics.rouge_n import RougeN
+from keras_nlp.src.metrics.rouge_l import RougeL
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
-class RougeNTest(TestCase):
+class RougeLTest(TestCase):
     def test_initialization(self):
-        rouge = RougeN()
+        rouge = RougeL()
         result = rouge.result()
 
-        self.assertAllClose(
+        self.assertDictEqual(
             result,
             {"precision": 0.0, "recall": 0.0, "f1_score": 0.0},
         )
 
     def test_string_input(self):
-        rouge = RougeN(order=2, use_stemmer=False)
+        rouge = RougeL(use_stemmer=False)
         y_true = "the tiny little cat was found under the big funny bed"
         y_pred = "the cat was under the bed"
 
         rouge_val = rouge(y_true, y_pred)
         self.assertAllClose(
             rouge_val,
-            {"precision": 0.4, "recall": 0.2, "f1_score": 0.266666},
+            {"precision": 1.0, "recall": 0.545454, "f1_score": 0.705882},
         )
 
     def test_string_list_input(self):
-        rouge = RougeN(order=2, use_stemmer=False)
+        rouge = RougeL(use_stemmer=False)
         y_true = [
             "the tiny little cat was found under the big funny bed",
             "i really love contributing to KerasNLP",
         ]
         y_pred = [
             "the cat was under the bed",
             "i love contributing to KerasNLP",
         ]
 
         rouge_val = rouge(y_true, y_pred)
         self.assertAllClose(
             rouge_val,
-            {"precision": 0.575, "recall": 0.4, "f1_score": 0.466666},
+            {"precision": 1.0, "recall": 0.689393, "f1_score": 0.807486},
         )
 
     def test_tensor_input(self):
-        rouge = RougeN(order=2, use_stemmer=False)
-        y_true = tf.constant(
-            [
-                "the tiny little cat was found under the big funny bed",
-                "i really love contributing to KerasNLP",
-            ]
-        )
-        y_pred = tf.constant(
-            ["the cat was under the bed", "i love contributing to KerasNLP"]
-        )
-
-        rouge_val = rouge(y_true, y_pred)
-        self.assertAllClose(
-            rouge_val,
-            {"precision": 0.575, "recall": 0.4, "f1_score": 0.466666},
-        )
-
-    def test_rank_2_input(self):
-        rouge = RougeN(order=2, use_stemmer=False)
-        y_true = tf.constant(
-            [
-                ["the tiny little cat was found under the big funny bed"],
-                ["i really love contributing to KerasNLP"],
-            ]
-        )
-        y_pred = tf.constant(
-            [["the cat was under the bed"], ["i love contributing to KerasNLP"]]
-        )
-
-        rouge_val = rouge(y_true, y_pred)
-        self.assertAllClose(
-            rouge_val,
-            {"precision": 0.575, "recall": 0.4, "f1_score": 0.466666},
-        )
-
-    def test_model_compile(self):
-        inputs = keras.Input(shape=(None,), dtype="string")
-        outputs = keras.layers.Identity()(inputs)
-        model = keras.Model(inputs, outputs)
-
-        model.compile(metrics=[RougeN()])
-
-        y_pred = x = tf.constant(["hello this is fun"])
-        y = tf.constant(["hello this is awesome"])
-
-        output = model.compute_metrics(x, y, y_pred, sample_weight=None)
-        self.assertAllClose(output["precision"], 0.666666)
-        self.assertAllClose(output["recall"], 0.666666)
-        self.assertAllClose(output["f1_score"], 0.666666)
-
-    def test_incorrect_order(self):
-        with self.assertRaises(ValueError):
-            _ = RougeN(order=10)
-
-    def test_different_order(self):
-        rouge = RougeN(order=3, use_stemmer=False)
+        rouge = RougeL(use_stemmer=False)
         y_true = tf.constant(
             [
                 "the tiny little cat was found under the big funny bed",
                 "i really love contributing to KerasNLP",
             ]
         )
         y_pred = tf.constant(
             ["the cat was under the bed", "i love contributing to KerasNLP"]
         )
 
         rouge_val = rouge(y_true, y_pred)
         self.assertAllClose(
             rouge_val,
-            {"precision": 0.333333, "recall": 0.25, "f1_score": 0.285714},
+            {"precision": 1.0, "recall": 0.689393, "f1_score": 0.807486},
         )
 
     def test_reset_state(self):
-        rouge = RougeN()
-        y_true = tf.constant(
-            ["hey, this is great fun", "i love contributing to KerasNLP"]
-        )
-        y_pred = tf.constant(
-            [
-                "great fun indeed",
-                "KerasNLP is awesome, i love contributing to it",
-            ]
-        )
+        rouge = RougeL()
+        y_true = ["hey, this is great fun", "i love contributing to KerasNLP"]
+        y_pred = [
+            "great fun indeed",
+            "KerasNLP is awesome, i love contributing to it",
+        ]
 
         rouge.update_state(y_true, y_pred)
         rouge_val = rouge.result()
         self.assertNotAllClose(
             rouge_val,
             {"precision": 0.0, "recall": 0.0, "f1_score": 0.0},
         )
 
         rouge.reset_state()
         rouge_val = rouge.result()
-        self.assertAllClose(
+        self.assertDictEqual(
             rouge_val,
             {"precision": 0.0, "recall": 0.0, "f1_score": 0.0},
         )
 
     def test_update_state(self):
-        rouge = RougeN()
-        y_true_1 = tf.constant(
-            [
-                "the tiny little cat was found under the big funny bed",
-                "i really love contributing to KerasNLP",
-            ]
-        )
-        y_pred_1 = tf.constant(
-            ["the cat was under the bed", "i love contributing to KerasNLP"]
-        )
+        rouge = RougeL()
+        y_true_1 = [
+            "the tiny little cat was found under the big funny bed",
+            "i really love contributing to KerasNLP",
+        ]
+        y_pred_1 = [
+            "the cat was under the bed",
+            "i love contributing to KerasNLP",
+        ]
 
         rouge.update_state(y_true_1, y_pred_1)
         rouge_val = rouge.result()
         self.assertAllClose(
             rouge_val,
-            {"precision": 0.575, "recall": 0.4, "f1_score": 0.466666},
+            {"precision": 1.0, "recall": 0.689393, "f1_score": 0.807486},
         )
 
-        y_true_2 = tf.constant(["what is your favourite show"])
-        y_pred_2 = tf.constant(["my favourite show is silicon valley"])
+        y_true_2 = ["what is your favourite show"]
+        y_pred_2 = ["my favourite show is silicon valley"]
 
         rouge.update_state(y_true_2, y_pred_2)
         rouge_val = rouge.result()
         self.assertAllClose(
             rouge_val,
-            {"precision": 0.45, "recall": 0.35, "f1_score": 0.385185},
+            {"precision": 0.777777, "recall": 0.592929, "f1_score": 0.659536},
         )
 
     def test_get_config(self):
-        rouge = RougeN(
-            order=5,
+        rouge = RougeL(
             use_stemmer=True,
             dtype="float32",
-            name="rouge_n_test",
+            name="rouge_l_test",
         )
 
         config = rouge.get_config()
         expected_config_subset = {
-            "order": 5,
             "use_stemmer": True,
         }
-
         self.assertEqual(config, {**config, **expected_config_subset})
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,21 @@
 from keras_nlp.src.models.gpt2.gpt2_causal_lm import GPT2CausalLM
 from keras_nlp.src.models.gpt2.gpt2_causal_lm_preprocessor import (
     GPT2CausalLMPreprocessor,
 )
 from keras_nlp.src.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
 from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_backbone import GPTNeoXBackbone
+from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_causal_lm import GPTNeoXCausalLM
+from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_causal_lm_preprocessor import (
+    GPTNeoXCausalLMPreprocessor,
+)
+from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_preprocessor import (
+    GPTNeoXPreprocessor,
+)
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_tokenizer import GPTNeoXTokenizer
 from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
 from keras_nlp.src.models.opt.opt_causal_lm import OPTCausalLM
 from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import (
     OPTCausalLMPreprocessor,
 )
 from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_backbone_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Test for ALBERT backbone model."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
 from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
 from keras_nlp.src.tests.test_case import TestCase
 
 
 class AlbertBackboneTest(TestCase):
     def setUp(self):
         self.backbone = AlbertBackbone(
@@ -35,17 +35,17 @@
             embedding_dim=16,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
         )
         self.batch_size = 8
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "segment_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "segment_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
 
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_valid_call_albert(self):
@@ -54,17 +54,17 @@
     def test_name(self):
         # Check default name passed through
         self.assertRegexpMatches(self.backbone.name, "albert_backbone")
 
     def test_variable_sequence_length_call_albert(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "segment_ids": ops.ones((2, seq_length), dtype="int32"),
-                "padding_mask": ops.ones((2, seq_length), dtype="int32"),
+                "token_ids": np.ones((2, seq_length), dtype="int32"),
+                "segment_ids": np.ones((2, seq_length), dtype="int32"),
+                "padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
             self.backbone(input_data)
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
@@ -118,17 +118,17 @@
                 embedding_dim=16,
                 hidden_dim=2,
                 intermediate_dim=2,
                 max_sequence_length=4,
             )
 
         self.input_batch = {
-            "token_ids": ops.ones((8, 128), dtype="int32"),
-            "segment_ids": ops.ones((8, 128), dtype="int32"),
-            "padding_mask": ops.ones((8, 128), dtype="int32"),
+            "token_ids": np.ones((8, 128), dtype="int32"),
+            "segment_ids": np.ones((8, 128), dtype="int32"),
+            "padding_mask": np.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_classifier.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_classifier_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_classifier_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for ALBERT classification model."""
 
 import io
 import os
 
+import numpy as np
 import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
@@ -80,15 +81,15 @@
 
         self.raw_batch = [
             "the quick brown fox.",
             "the slow brown fox.",
         ]
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, ops.ones((2,)))
+            (self.raw_batch, np.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
     def test_classifier_predict(self):
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_masked_lm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for ALBERT masked language model preprocessor layer."""
 
 import io
-import os
 
-import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.albert.albert_masked_lm_preprocessor import (
     AlbertMaskedLMPreprocessor,
 )
@@ -53,15 +51,15 @@
 
         proto = bytes_io.getvalue()
 
         tokenizer = AlbertTokenizer(proto=proto)
 
         self.preprocessor = AlbertMaskedLMPreprocessor(
             tokenizer=tokenizer,
-            # Simplify out testing by masking every available token.
+            # Simplify our testing by masking every available token.
             mask_selection_rate=1.0,
             mask_token_rate=1.0,
             random_token_rate=0.0,
             mask_selection_length=4,
             sequence_length=12,
         )
 
@@ -147,24 +145,7 @@
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs, y, sw = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        outputs = model(input_data)["token_ids"]
-        restored_outputs = restored_model(input_data)["token_ids"]
-        self.assertAllEqual(outputs, restored_outputs)
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_masked_lm_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_masked_lm_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         proto = bytes_io.getvalue()
 
         tokenizer = AlbertTokenizer(proto=proto)
 
         self.preprocessor = AlbertMaskedLMPreprocessor(
             tokenizer=tokenizer,
-            # Simplify out testing by masking every available token.
+            # Simplify our testing by masking every available token.
             mask_selection_rate=1.0,
             mask_token_rate=1.0,
             random_token_rate=0.0,
             mask_selection_length=5,
             sequence_length=5,
         )
         self.backbone = AlbertBackbone(
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_preprocessor_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for ALBERT preprocessor layer."""
 import io
-import os
 
-import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
 from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
 from keras_nlp.src.tests.test_case import TestCase
@@ -161,22 +159,7 @@
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/albert/albert_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,103 +8,95 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for ALBERT tokenizer."""
+"""Tests for DeBERTa tokenizer."""
 import io
-import os
 
-import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class AlbertTokenizerTest(TestCase):
+class DebertaV3TokenizerTest(TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
-            vocab_size=12,
+            vocab_size=10,
             model_type="WORD",
             pad_id=0,
-            unk_id=1,
-            bos_id=2,
-            eos_id=3,
-            pad_piece="<pad>",
-            unk_piece="<unk>",
+            bos_id=1,
+            eos_id=2,
+            unk_id=3,
+            pad_piece="[PAD]",
             bos_piece="[CLS]",
             eos_piece="[SEP]",
-            user_defined_symbols="[MASK]",
+            unk_piece="[UNK]",
         )
         self.proto = bytes_io.getvalue()
 
-        self.tokenizer = AlbertTokenizer(proto=self.proto)
+        self.tokenizer = DebertaV3Tokenizer(proto=self.proto)
 
     def test_tokenize(self):
         input_data = "the quick brown fox"
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [5, 10, 6, 8])
+        self.assertAllEqual(output, [4, 9, 5, 7])
 
     def test_tokenize_batch(self):
         input_data = ["the quick brown fox", "the earth is round"]
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [[5, 10, 6, 8], [5, 7, 9, 11]])
+        self.assertAllEqual(output, [[4, 9, 5, 7], [4, 6, 8, 3]])
 
     def test_detokenize(self):
-        input_data = [[5, 10, 6, 8]]
+        input_data = [[4, 9, 5, 7]]
+        output = self.tokenizer.detokenize(input_data)
+        self.assertEqual(output, ["the quick brown fox"])
+
+    def test_detokenize_mask_token(self):
+        input_data = [[4, 9, 5, 7, self.tokenizer.mask_token_id]]
         output = self.tokenizer.detokenize(input_data)
         self.assertEqual(output, ["the quick brown fox"])
 
     def test_vocabulary_size(self):
-        tokenizer = AlbertTokenizer(proto=self.proto)
-        self.assertEqual(tokenizer.vocabulary_size(), 12)
+        self.assertEqual(self.tokenizer.vocabulary_size(), 11)
+
+    def test_get_vocabulary_mask_token(self):
+        self.assertEqual(self.tokenizer.get_vocabulary()[10], "[MASK]")
+
+    def test_id_to_token_mask_token(self):
+        self.assertEqual(self.tokenizer.id_to_token(10), "[MASK]")
+
+    def test_token_to_id_mask_token(self):
+        self.assertEqual(self.tokenizer.token_to_id("[MASK]"), 10)
 
     def test_errors_missing_special_tokens(self):
         bytes_io = io.BytesIO()
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=iter(["abc"]),
             model_writer=bytes_io,
             vocab_size=5,
             pad_id=-1,
             eos_id=-1,
             bos_id=-1,
         )
         with self.assertRaises(ValueError):
-            AlbertTokenizer(proto=bytes_io.getvalue())
+            DebertaV3Tokenizer(proto=bytes_io.getvalue())
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.tokenizer)
         new_tokenizer = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_tokenizer.get_config(),
             self.tokenizer.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_backbone_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Test for BART backbone models."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
 from keras_nlp.src.models.bart.bart_backbone import BartBackbone
 from keras_nlp.src.tests.test_case import TestCase
 
 
 class BartBackboneTest(TestCase):
     def setUp(self):
         self.backbone = BartBackbone(
@@ -31,18 +31,18 @@
             num_layers=2,
             num_heads=2,
             hidden_dim=3,
             intermediate_dim=4,
             max_sequence_length=5,
         )
         self.input_batch = {
-            "encoder_token_ids": ops.ones((2, 5), dtype="int32"),
-            "encoder_padding_mask": ops.ones((2, 5), dtype="int32"),
-            "decoder_token_ids": ops.ones((2, 5), dtype="int32"),
-            "decoder_padding_mask": ops.ones((2, 5), dtype="int32"),
+            "encoder_token_ids": np.ones((2, 5), dtype="int32"),
+            "encoder_padding_mask": np.ones((2, 5), dtype="int32"),
+            "decoder_token_ids": np.ones((2, 5), dtype="int32"),
+            "decoder_padding_mask": np.ones((2, 5), dtype="int32"),
         }
 
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_valid_call(self):
@@ -51,22 +51,18 @@
     def test_name(self):
         # Check default name passed through
         self.assertRegexpMatches(self.backbone.name, "bart_backbone")
 
     def test_variable_sequence_length_call(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "encoder_token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "encoder_padding_mask": ops.ones(
-                    (2, seq_length), dtype="int32"
-                ),
-                "decoder_token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "decoder_padding_mask": ops.ones(
-                    (2, seq_length), dtype="int32"
-                ),
+                "encoder_token_ids": np.ones((2, seq_length), dtype="int32"),
+                "encoder_padding_mask": np.ones((2, seq_length), dtype="int32"),
+                "decoder_token_ids": np.ones((2, seq_length), dtype="int32"),
+                "decoder_padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
             self.backbone(input_data)
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
@@ -108,18 +104,18 @@
                 num_layers=2,
                 num_heads=2,
                 hidden_dim=64,
                 intermediate_dim=128,
                 max_sequence_length=128,
             )
         self.input_batch = {
-            "encoder_token_ids": ops.ones((8, 128), dtype="int32"),
-            "encoder_padding_mask": ops.ones((8, 128), dtype="int32"),
-            "decoder_token_ids": ops.ones((8, 128), dtype="int32"),
-            "decoder_padding_mask": ops.ones((8, 128), dtype="int32"),
+            "encoder_token_ids": np.ones((8, 128), dtype="int32"),
+            "encoder_padding_mask": np.ones((8, 128), dtype="int32"),
+            "decoder_token_ids": np.ones((8, 128), dtype="int32"),
+            "decoder_padding_mask": np.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_preprocessor_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for BART preprocessor layer."""
-import os
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.bart.bart_preprocessor import BartPreprocessor
 from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
@@ -163,39 +161,7 @@
         new_preprocessor = keras.saving.deserialize_keras_object(
             keras.saving.serialize_keras_object(self.preprocessor)
         )
         self.assertEqual(
             new_preprocessor.get_config(), self.preprocessor.get_config()
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = {
-            "encoder_text": tf.constant([" airplane at airport"]),
-            "decoder_text": tf.constant([" kohli is the best"]),
-        }
-
-        inputs = {
-            "encoder_text": keras.Input(
-                dtype="string", name="encoder_text", shape=()
-            ),
-            "decoder_text": keras.Input(
-                dtype="string", name="decoder_text", shape=()
-            ),
-        }
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs=inputs, outputs=outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-
-        model_output = model(input_data)
-        restored_model_output = restored_model(input_data)
-
-        self.assertAllClose(
-            model_output,
-            restored_model_output,
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,16 +522,17 @@
             hidden_states=hidden_states,
         )
 
         # Compute an output padding mask with the token ids we updated.
         if end_token_id is not None:
             # Build a mask of `end_token_id` locations not in the original
             # prompt (not in locations where `decoder_padding_mask` is True).
-            end_locations = (decoder_token_ids == end_token_id) & (
-                ~decoder_padding_mask
+            end_locations = ops.logical_and(
+                ops.equal(decoder_token_ids, end_token_id),
+                ops.logical_not(decoder_padding_mask),
             )
             end_locations = ops.cast(end_locations, "int32")
             # Use cumsum to get ones in all locations after `end_locations`.
             cumsum = ops.cast(ops.cumsum(end_locations, axis=-1), "int32")
             overflow = cumsum - end_locations
             # Our padding mask is the inverse of these overflow locations.
             decoder_padding_mask = ops.logical_not(ops.cast(overflow, "bool"))
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_preprocessor_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,182 +8,179 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for BART preprocessor layer."""
-import os
+"""Tests for Whisper preprocessor layer."""
+
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.bart.bart_seq_2_seq_lm_preprocessor import (
-    BartSeq2SeqLMPreprocessor,
+from keras_nlp.src.models.whisper.whisper_audio_feature_extractor import (
+    WhisperAudioFeatureExtractor,
 )
-from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
+from keras_nlp.src.models.whisper.whisper_preprocessor import WhisperPreprocessor
+from keras_nlp.src.models.whisper.whisper_tokenizer import WhisperTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class BartSeq2SeqLMPreprocessorTest(TestCase):
+class WhisperPreprocessorTest(TestCase):
     def setUp(self):
-        vocab = {
-            "<s>": 0,
-            "<pad>": 1,
-            "</s>": 2,
-            "Ġair": 3,
-            "plane": 4,
-            "Ġat": 5,
-            "port": 6,
-            "Ġkoh": 7,
-            "li": 8,
-            "Ġis": 9,
-            "Ġthe": 10,
-            "Ġbest": 11,
-            "<mask>": 12,
+        self.num_mels = 80
+        self.num_fft_bins = 400
+        self.stride = 100
+        self.sampling_rate = 100
+        self.max_audio_length = 5
+        self.output_length = (
+            self.max_audio_length * self.sampling_rate
+        ) // self.stride
+        self.audio_feature_extractor = WhisperAudioFeatureExtractor(
+            num_mels=self.num_mels,
+            num_fft_bins=self.num_fft_bins,
+            stride=self.stride,
+            sampling_rate=self.sampling_rate,
+            max_audio_length=self.max_audio_length,
+        )
+
+        self.vocab = {
+            "Ġair": 0,
+            "plane": 1,
+            "Ġat": 2,
+            "port": 3,
+            "Ġkoh": 4,
+            "li": 5,
+            "Ġis": 6,
+            "Ġthe": 7,
+            "Ġbest": 8,
         }
 
         merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
         merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
         merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
         merges += ["pla ne"]
+        self.merges = merges
+
+        self.special_tokens = {
+            "<|startoftranscript|>": 9,
+            "<|endoftext|>": 10,
+            "<|notimestamps|>": 11,
+            "<|transcribe|>": 12,
+            "<|translate|>": 13,
+        }
+
+        self.language_tokens = {
+            "<|en|>": 14,
+            "<|fr|>": 15,
+        }
 
-        self.preprocessor = BartSeq2SeqLMPreprocessor(
-            tokenizer=BartTokenizer(
-                vocabulary=vocab,
-                merges=merges,
-            ),
-            encoder_sequence_length=10,
-            decoder_sequence_length=9,
+        self.tokenizer = WhisperTokenizer(
+            vocabulary=self.vocab,
+            merges=self.merges,
+            special_tokens=self.special_tokens,
+            language_tokens=self.language_tokens,
         )
 
-    def test_tokenize_strings(self):
+        self.preprocessor = WhisperPreprocessor(
+            audio_feature_extractor=self.audio_feature_extractor,
+            tokenizer=self.tokenizer,
+            decoder_sequence_length=12,
+            language="<|en|>",
+            task="translate",
+        )
+
+    def test_unbatched_preprocess(self):
         input_data = {
-            "encoder_text": " airplane at airport",
-            "decoder_text": " kohli is the best",
+            "encoder_audio": tf.ones((200,)),
+            "decoder_text": tf.constant(" airplane at airport"),
         }
 
-        x_out, y_out, sw_out = self.preprocessor(input_data)
-        self.assertAllEqual(
-            x_out["encoder_token_ids"], [0, 3, 4, 5, 3, 6, 2, 1, 1, 1]
-        )
+        x = self.preprocessor(input_data)
         self.assertAllEqual(
-            x_out["encoder_padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0]
+            x["encoder_features"].shape, [self.output_length, self.num_mels]
         )
         self.assertAllEqual(
-            x_out["decoder_token_ids"], [2, 0, 7, 8, 9, 10, 11, 2, 1]
+            x["decoder_token_ids"], [9, 14, 13, 11, 0, 1, 2, 0, 3, 10, 10, 10]
         )
         self.assertAllEqual(
-            x_out["decoder_padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 0]
+            x["decoder_padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]
         )
-        self.assertAllEqual(y_out, [0, 7, 8, 9, 10, 11, 2, 1, 1])
-        self.assertAllEqual(sw_out, [1, 1, 1, 1, 1, 1, 1, 0, 0])
 
-    def test_tokenize_list_of_strings(self):
+    def test_preprocess_batch(self):
         input_data = {
-            "encoder_text": [" airplane at airport"] * 4,
-            "decoder_text": [" kohli is the best"] * 4,
+            "encoder_audio": tf.ones((4, 200)),
+            "decoder_text": tf.constant([" airplane at airport"] * 4),
         }
 
-        x_out, y_out, sw_out = self.preprocessor(input_data)
+        x = self.preprocessor(input_data)
         self.assertAllEqual(
-            x_out["encoder_token_ids"], [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1]] * 4
+            x["encoder_features"].shape, [4, self.output_length, self.num_mels]
         )
         self.assertAllEqual(
-            x_out["encoder_padding_mask"],
-            [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0]] * 4,
+            x["decoder_token_ids"],
+            [[9, 14, 13, 11, 0, 1, 2, 0, 3, 10, 10, 10]] * 4,
         )
         self.assertAllEqual(
-            x_out["decoder_token_ids"], [[2, 0, 7, 8, 9, 10, 11, 2, 1]] * 4
+            x["decoder_padding_mask"],
+            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 4,
         )
-        self.assertAllEqual(
-            x_out["decoder_padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 0]] * 4
-        )
-        self.assertAllEqual(y_out, [[0, 7, 8, 9, 10, 11, 2, 1, 1]] * 4)
-        self.assertAllEqual(sw_out, [[1, 1, 1, 1, 1, 1, 1, 0, 0]] * 4)
-
-    def test_error_multi_segment_input(self):
-        input_data = {
-            "encoder_text": (
-                tf.constant([" airplane at airport"] * 2),
-                tf.constant([" airplane"] * 2),
-            ),
-            "decoder_text": (
-                tf.constant([" kohli is the best"] * 2),
-                tf.constant([" kohli"] * 2),
-            ),
-        }
-
-        with self.assertRaises(ValueError):
-            self.preprocessor(input_data)
 
-    def test_generate_preprocess(self):
-        input_data = {
-            "encoder_text": tf.convert_to_tensor([" airplane at airport"]),
-            "decoder_text": tf.convert_to_tensor([" kohli is the best"]),
+    def test_preprocess_labeled_batch(self):
+        x = {
+            "encoder_audio": tf.ones((4, 200)),
+            "decoder_text": tf.constant([" airplane at airport"] * 4),
         }
-        x_out = self.preprocessor.generate_preprocess(input_data)
+        y_in = tf.constant([1] * 4)
+        sw_in = tf.constant([1.0] * 4)
+        x, y, sw = self.preprocessor(x, y_in, sw_in)
         self.assertAllEqual(
-            x_out["encoder_token_ids"], [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1]]
+            x["encoder_features"].shape, [4, self.output_length, self.num_mels]
         )
         self.assertAllEqual(
-            x_out["encoder_padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0]]
+            x["decoder_token_ids"],
+            [[9, 14, 13, 11, 0, 1, 2, 0, 3, 10, 10, 10]] * 4,
         )
         self.assertAllEqual(
-            x_out["decoder_token_ids"], [[2, 0, 7, 8, 9, 10, 11, 1, 1]]
-        )
-        self.assertAllEqual(
-            x_out["decoder_padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0]]
+            x["decoder_padding_mask"],
+            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 4,
         )
+        self.assertAllEqual(y, y_in)
+        self.assertAllEqual(sw, sw_in)
 
-    def test_generate_postprocess(self):
-        input_data = {
-            "decoder_token_ids": tf.constant([2, 0, 7, 8, 9, 10, 11, 1, 1]),
-            "decoder_padding_mask": tf.cast(
-                [1, 1, 1, 1, 1, 1, 1, 0, 0], dtype="bool"
-            ),
+    def test_preprocess_dataset(self):
+        x = {
+            "encoder_audio": tf.ones((4, 200)),
+            "decoder_text": tf.constant([" airplane at airport"] * 4),
         }
-        x = self.preprocessor.generate_postprocess(input_data)
-        self.assertAllEqual(x, " kohli is the best")
-
-    def test_serialization(self):
-        new_preprocessor = keras.saving.deserialize_keras_object(
-            keras.saving.serialize_keras_object(self.preprocessor)
+        ds = tf.data.Dataset.from_tensor_slices(x)
+        ds = ds.map(self.preprocessor)
+        x = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(
+            x["encoder_features"].shape, [4, self.output_length, self.num_mels]
         )
-        self.assertEqual(
-            new_preprocessor.get_config(), self.preprocessor.get_config()
+        self.assertAllEqual(
+            x["decoder_token_ids"],
+            [[9, 14, 13, 11, 0, 1, 2, 0, 3, 10, 10, 10]] * 4,
+        )
+        self.assertAllEqual(
+            x["decoder_padding_mask"],
+            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 4,
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
+    def test_sequence_length_override(self):
         input_data = {
-            "encoder_text": tf.constant([" airplane at airport"]),
-            "decoder_text": tf.constant([" kohli is the best"]),
-        }
-
-        inputs = {
-            "encoder_text": keras.Input(
-                dtype="string", name="encoder_text", shape=()
-            ),
-            "decoder_text": keras.Input(
-                dtype="string", name="decoder_text", shape=()
-            ),
+            "encoder_audio": tf.ones((200,)),
+            "decoder_text": tf.constant(" airplane at airport"),
         }
-        outputs, y, sw = self.preprocessor(inputs)
-        model = keras.Model(inputs=inputs, outputs=outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
+        x = self.preprocessor(input_data, decoder_sequence_length=6)
+        self.assertAllEqual(x["decoder_token_ids"], [9, 14, 13, 11, 0, 10])
 
-        restored_model = keras.models.load_model(path)
-
-        model_output = model(input_data)
-        restored_model_output = restored_model(input_data)
-
-        self.assertAllClose(
-            model_output,
-            restored_model_output,
+    def test_serialization(self):
+        config = keras.saving.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.saving.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
         )
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bart/bart_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_tokenizer_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for BART tokenizer."""
-import os
 
-import pytest
-import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
 class BartTokenizerTest(TestCase):
@@ -78,25 +75,7 @@
         config = keras.saving.serialize_keras_object(self.tokenizer)
         new_tokenizer = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_tokenizer.get_config(),
             self.tokenizer.get_config(),
         )
 
-    @pytest.mark.large  # Saving is slow, so mark these large.
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant([" airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,63 +7,61 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for BERT backbone models."""
+"""Test for DistilBERT backbone models."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
-from keras_nlp.src.models.bert.bert_backbone import BertBackbone
+from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class BertBackboneTest(TestCase):
+class DistilBertTest(TestCase):
     def setUp(self):
-        self.backbone = BertBackbone(
+        self.backbone = DistilBertBackbone(
             vocabulary_size=10,
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
+            name="encoder",
         )
+
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "segment_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
+
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
-    def test_valid_call_bert(self):
+    def test_valid_call_distilbert(self):
         self.backbone(self.input_batch)
 
     def test_token_embedding(self):
         output = self.backbone.token_embedding(self.input_batch["token_ids"])
         self.assertEqual(output.shape, (2, 5, 2))
 
-    def test_name(self):
-        # Check default name passed through
-        self.assertRegexpMatches(self.backbone.name, "bert_backbone")
-
-    def test_variable_sequence_length_call_bert(self):
+    def test_variable_sequence_length_call_distilbert(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "segment_ids": ops.ones((2, seq_length), dtype="int32"),
-                "padding_mask": ops.ones((2, seq_length), dtype="int32"),
+                "token_ids": np.ones((2, seq_length), dtype="int32"),
+                "mask_positions": np.ones((2, seq_length), dtype="int32"),
+                "padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
             self.backbone(input_data)
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
@@ -77,38 +75,37 @@
     def test_saved_model(self):
         model_output = self.backbone(self.input_batch)
         path = os.path.join(self.get_temp_dir(), "model.keras")
         self.backbone.save(path, save_format="keras_v3")
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, BertBackbone)
+        self.assertIsInstance(restored_model, DistilBertBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
         self.assertAllClose(model_output, restored_output)
 
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
-class BertBackboneTPUTest(TestCase):
+class DistilBertTPUTest(TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
-            self.backbone = BertBackbone(
+            self.backbone = DistilBertBackbone(
                 vocabulary_size=1000,
                 num_layers=2,
                 num_heads=2,
                 hidden_dim=64,
                 intermediate_dim=128,
                 max_sequence_length=128,
             )
         self.input_batch = {
-            "token_ids": ops.ones((8, 128), dtype="int32"),
-            "segment_ids": ops.ones((8, 128), dtype="int32"),
-            "padding_mask": ops.ones((8, 128), dtype="int32"),
+            "token_ids": np.ones((8, 128), dtype="int32"),
+            "padding_mask": np.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_classifier.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_classifier_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_classifier_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for BERT classification model."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.bert.bert_backbone import BertBackbone
 from keras_nlp.src.models.bert.bert_classifier import BertClassifier
@@ -55,15 +56,15 @@
         # Setup data.
         self.raw_batch = [
             "the quick brown fox.",
             "the slow brown fox.",
         ]
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, ops.ones((2,)))
+            (self.raw_batch, np.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
     def test_classifier_predict(self):
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_masked_lm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,154 +1,150 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for BERT masked language model preprocessor layer."""
 
-import os
+"""Tests for XLM-RoBERTa masked language model preprocessor layer."""
+import io
 
-import pytest
+import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.bert.bert_masked_lm_preprocessor import (
-    BertMaskedLMPreprocessor,
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
+    XLMRobertaMaskedLMPreprocessor,
+)
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
+    XLMRobertaTokenizer,
 )
-from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class BertMaskedLMPreprocessorTest(TestCase):
+class XLMRobertaMaskedLMPreprocessorTest(TestCase):
     def setUp(self):
-        self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
-        self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
-        self.vocab += ["the", "quick", "brown", "fox"]
-
-        tokenizer = BertTokenizer(vocabulary=self.vocab)
-
-        self.preprocessor = BertMaskedLMPreprocessor(
-            tokenizer=tokenizer,
-            # Simplify out testing by masking every available token.
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the earth is round"]
+        )
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=12,
+            model_type="WORD",
+            pad_id=0,
+            unk_id=1,
+            bos_id=2,
+            eos_id=3,
+            pad_piece="<pad>",
+            unk_piece="<unk>",
+            bos_piece="<s>",
+            eos_piece="</s>",
+            user_defined_symbols="[MASK]",
+        )
+        self.proto = bytes_io.getvalue()
+
+        self.tokenizer = XLMRobertaTokenizer(proto=self.proto)
+        self.preprocessor = XLMRobertaMaskedLMPreprocessor(
+            tokenizer=self.tokenizer,
+            # Simplify our testing by masking every available token.
             mask_selection_rate=1.0,
             mask_token_rate=1.0,
             random_token_rate=0.0,
-            mask_selection_length=4,
+            mask_selection_length=5,
             sequence_length=12,
         )
 
     def test_preprocess_strings(self):
-        input_data = "the quick brown fox"
+        input_data = " brown fox quick"
 
         x, y, sw = self.preprocessor(input_data)
         self.assertAllEqual(
-            x["token_ids"], [2, 4, 4, 4, 4, 3, 0, 0, 0, 0, 0, 0]
-        )
-        self.assertAllEqual(
-            x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
+            x["token_ids"], [0, 13, 13, 13, 2, 1, 1, 1, 1, 1, 1, 1]
         )
         self.assertAllEqual(
-            x["segment_ids"], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+            x["padding_mask"], [1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]
         )
-        self.assertAllEqual(x["mask_positions"], [1, 2, 3, 4])
-        self.assertAllEqual(y, [9, 10, 11, 12])
-        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0])
+        self.assertAllEqual(x["mask_positions"], [1, 2, 3, 0, 0])
+        self.assertAllEqual(y, [7, 9, 11, 0, 0])
+        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 0.0, 0.0])
 
     def test_preprocess_list_of_strings(self):
-        input_data = ["the quick brown fox"] * 4
+        input_data = [" brown fox quick"] * 13
 
         x, y, sw = self.preprocessor(input_data)
         self.assertAllEqual(
-            x["token_ids"], [[2, 4, 4, 4, 4, 3, 0, 0, 0, 0, 0, 0]] * 4
+            x["token_ids"], [[0, 13, 13, 13, 2, 1, 1, 1, 1, 1, 1, 1]] * 13
         )
         self.assertAllEqual(
-            x["padding_mask"],
-            [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4,
+            x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]] * 13
         )
-        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4]] * 4)
-        self.assertAllEqual(y, [[9, 10, 11, 12]] * 4)
-        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0]] * 4)
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 0, 0]] * 13)
+        self.assertAllEqual(y, [[7, 9, 11, 0, 0]] * 13)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 0.0, 0.0]] * 13)
 
     def test_preprocess_dataset(self):
-        sentences = tf.constant(["the quick brown fox"] * 4)
+        sentences = tf.constant([" brown fox quick"] * 13)
         ds = tf.data.Dataset.from_tensor_slices(sentences)
         ds = ds.map(self.preprocessor)
-        x, y, sw = ds.batch(4).take(1).get_single_element()
+        x, y, sw = ds.batch(13).take(1).get_single_element()
         self.assertAllEqual(
-            x["token_ids"], [[2, 4, 4, 4, 4, 3, 0, 0, 0, 0, 0, 0]] * 4
+            x["token_ids"], [[0, 13, 13, 13, 2, 1, 1, 1, 1, 1, 1, 1]] * 13
         )
         self.assertAllEqual(
-            x["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
+            x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]] * 13
         )
-        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4]] * 4)
-        self.assertAllEqual(y, [[9, 10, 11, 12]] * 4)
-        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0]] * 4)
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 0, 0]] * 13)
+        self.assertAllEqual(y, [[7, 9, 11, 0, 0]] * 13)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 0.0, 0.0]] * 13)
 
     def test_mask_multiple_sentences(self):
-        sentence_one = tf.constant("the quick")
-        sentence_two = tf.constant("brown fox")
+        sentence_one = tf.constant(" airplane")
+        sentence_two = tf.constant(" round")
 
         x, y, sw = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
-            x["token_ids"], [2, 4, 4, 3, 4, 4, 3, 0, 0, 0, 0, 0]
+            x["token_ids"], [0, 2, 2, 2, 13, 2, 1, 1, 1, 1, 1, 1]
         )
         self.assertAllEqual(
-            x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]
+            x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
         )
-        self.assertAllEqual(x["mask_positions"], [1, 2, 4, 5])
-        self.assertAllEqual(y, [9, 10, 11, 12])
-        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0])
+        self.assertAllEqual(x["mask_positions"], [4, 0, 0, 0, 0])
+        self.assertAllEqual(y, [12, 0, 0, 0, 0])
+        self.assertAllEqual(sw, [1.0, 0.0, 0.0, 0.0, 0.0])
 
     def test_no_masking_zero_rate(self):
-        no_mask_preprocessor = BertMaskedLMPreprocessor(
+        no_mask_preprocessor = XLMRobertaMaskedLMPreprocessor(
             self.preprocessor.tokenizer,
             mask_selection_rate=0.0,
-            mask_selection_length=4,
+            mask_selection_length=5,
             sequence_length=12,
         )
-        input_data = "the quick brown fox"
+        input_data = " quick brown fox"
 
         x, y, sw = no_mask_preprocessor(input_data)
         self.assertAllEqual(
-            x["token_ids"], [2, 9, 10, 11, 12, 3, 0, 0, 0, 0, 0, 0]
+            x["token_ids"], [0, 11, 7, 9, 2, 1, 1, 1, 1, 1, 1, 1]
         )
         self.assertAllEqual(
-            x["padding_mask"],
-            [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0],
+            x["padding_mask"], [1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]
         )
-        self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0])
-        self.assertAllEqual(y, [0, 0, 0, 0])
-        self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0])
+        self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0, 0])
+        self.assertAllEqual(y, [0, 0, 0, 0, 0])
+        self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0, 0.0])
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large  # Saving is slow, so mark these large.
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs, y, sw = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        outputs = model(input_data)["token_ids"]
-        restored_outputs = restored_model(input_data)["token_ids"]
-        self.assertAllEqual(outputs, restored_outputs)
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_masked_lm_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_masked_lm_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 class BertMaskedLMTest(TestCase):
     def setUp(self):
         # Setup model.
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["the", "quick", "brown", "fox", "."]
         self.preprocessor = BertMaskedLMPreprocessor(
             BertTokenizer(vocabulary=self.vocab),
-            # Simplify out testing by masking every available token.
+            # Simplify our testing by masking every available token.
             mask_selection_rate=1.0,
             mask_token_rate=1.0,
             random_token_rate=0.0,
-            mask_selection_length=2,
+            mask_selection_length=5,
             sequence_length=5,
         )
         self.backbone = BertBackbone(
             vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,108 +7,130 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for BERT preprocessor layer."""
 
-import os
+"""Tests for DeBERTa preprocessor layer."""
+import io
 
-import pytest
+import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
-from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import (
+    DebertaV3Preprocessor,
+)
+from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class BertPreprocessorTest(TestCase):
+class DebertaV3PreprocessorTest(TestCase):
     def setUp(self):
-        self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
-        self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
-        self.vocab += ["the", "quick", "brown", "fox"]
-        self.preprocessor = BertPreprocessor(
-            BertTokenizer(vocabulary=self.vocab),
-            sequence_length=8,
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the earth is round"]
+        )
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=12,
+            model_type="WORD",
+            pad_id=0,
+            bos_id=1,
+            eos_id=2,
+            unk_id=3,
+            pad_piece="[PAD]",
+            bos_piece="[CLS]",
+            eos_piece="[SEP]",
+            unk_piece="[UNK]",
+            user_defined_symbols="[MASK]",
+        )
+        self.proto = bytes_io.getvalue()
+
+        self.preprocessor = DebertaV3Preprocessor(
+            tokenizer=DebertaV3Tokenizer(proto=self.proto),
+            sequence_length=12,
         )
 
     def test_tokenize_strings(self):
-        input_data = "THE QUICK BROWN FOX."
+        input_data = "the quick brown fox"
         output = self.preprocessor(input_data)
-        self.assertAllEqual(output["token_ids"], [2, 5, 6, 7, 8, 1, 3, 0])
-        self.assertAllEqual(output["segment_ids"], [0, 0, 0, 0, 0, 0, 0, 0])
-        self.assertAllEqual(output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
+        self.assertAllEqual(
+            output["token_ids"], [1, 5, 10, 6, 8, 2, 0, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(
+            output["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
+        )
 
     def test_tokenize_list_of_strings(self):
         # We should handle a list of strings as as batch.
-        input_data = ["THE QUICK BROWN FOX."] * 4
+        input_data = ["the quick brown fox"] * 4
         output = self.preprocessor(input_data)
-        self.assertAllEqual(output["token_ids"], [[2, 5, 6, 7, 8, 1, 3, 0]] * 4)
         self.assertAllEqual(
-            output["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0]] * 4
+            output["token_ids"], [[1, 5, 10, 6, 8, 2, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4
+            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
 
     def test_tokenize_labeled_batch(self):
-        x = tf.constant(["THE QUICK BROWN FOX."] * 4)
+        x = tf.constant(["the quick brown fox"] * 4)
         y = tf.constant([1] * 4)
         sw = tf.constant([1.0] * 4)
         x_out, y_out, sw_out = self.preprocessor(x, y, sw)
-        self.assertAllEqual(x_out["token_ids"], [[2, 5, 6, 7, 8, 1, 3, 0]] * 4)
         self.assertAllEqual(
-            x_out["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0]] * 4
+            x_out["token_ids"], [[1, 5, 10, 6, 8, 2, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(
-            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4
+            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(y_out, y)
         self.assertAllEqual(sw_out, sw)
 
     def test_tokenize_labeled_dataset(self):
-        x = tf.constant(["THE QUICK BROWN FOX."] * 4)
+        x = tf.constant(["the quick brown fox"] * 4)
         y = tf.constant([1] * 4)
         sw = tf.constant([1.0] * 4)
         ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
         ds = ds.map(self.preprocessor)
         x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
-        self.assertAllEqual(x_out["token_ids"], [[2, 5, 6, 7, 8, 1, 3, 0]] * 4)
         self.assertAllEqual(
-            x_out["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0]] * 4
+            x_out["token_ids"], [[1, 5, 10, 6, 8, 2, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(
-            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4
+            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(y_out, y)
         self.assertAllEqual(sw_out, sw)
 
     def test_tokenize_multiple_sentences(self):
-        sentence_one = tf.constant("THE QUICK")
-        sentence_two = tf.constant("BROWN FOX.")
+        sentence_one = tf.constant("the quick brown fox")
+        sentence_two = tf.constant("the earth")
         output = self.preprocessor((sentence_one, sentence_two))
-        self.assertAllEqual(output["token_ids"], [2, 5, 6, 3, 7, 8, 1, 3])
-        self.assertAllEqual(output["segment_ids"], [0, 0, 0, 0, 1, 1, 1, 1])
-        self.assertAllEqual(output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1])
+        self.assertAllEqual(
+            output["token_ids"], [1, 5, 10, 6, 8, 2, 5, 7, 2, 0, 0, 0]
+        )
+        self.assertAllEqual(
+            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]
+        )
 
     def test_tokenize_multiple_batched_sentences(self):
-        sentence_one = tf.constant(["THE QUICK"] * 4)
-        sentence_two = tf.constant(["BROWN FOX."] * 4)
+        sentence_one = tf.constant(["the quick brown fox"] * 4)
+        sentence_two = tf.constant(["the earth"] * 4)
         # The first tuple or list is always interpreted as an enumeration of
         # separate sequences to concatenate.
         output = self.preprocessor((sentence_one, sentence_two))
-        self.assertAllEqual(output["token_ids"], [[2, 5, 6, 3, 7, 8, 1, 3]] * 4)
         self.assertAllEqual(
-            output["segment_ids"], [[0, 0, 0, 0, 1, 1, 1, 1]] * 4
+            output["token_ids"], [[1, 5, 10, 6, 8, 2, 5, 7, 2, 0, 0, 0]] * 4
         )
         self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1]] * 4
+            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]] * 4
         )
 
     def test_errors_for_2d_list_input(self):
         ambiguous_input = [["one", "two"], ["three", "four"]]
         with self.assertRaises(ValueError):
             self.preprocessor(ambiguous_input)
 
@@ -116,22 +138,7 @@
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large  # Saving is slow, so mark these large.
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["THE QUICK BROWN FOX."])
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/bert/bert_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_tokenizer_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for BERT tokenizer."""
 
-import os
-
-import pytest
-import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
 class BertTokenizerTest(TestCase):
@@ -62,23 +58,7 @@
         config = keras.saving.serialize_keras_object(self.tokenizer)
         new_tokenizer = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_tokenizer.get_config(),
             self.tokenizer.get_config(),
         )
 
-    @pytest.mark.large  # Saving is slow, so mark these large.
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["THE QUICK BROWN FOX."])
-        tokenizer = BertTokenizer(vocabulary=self.vocab)
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
 from keras_nlp.src.models.deberta_v3.disentangled_attention_encoder import (
     DisentangledAttentionEncoder,
 )
 from keras_nlp.src.models.deberta_v3.relative_embedding import RelativeEmbedding
 from keras_nlp.src.utils.python_utils import classproperty
-from keras_nlp.src.utils.tensor_utils import assert_tf_backend
 
 
 def deberta_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3Backbone")
@@ -106,16 +105,14 @@
         hidden_dim,
         intermediate_dim,
         dropout=0.1,
         max_sequence_length=512,
         bucket_size=256,
         **kwargs,
     ):
-        assert_tf_backend(self.__class__.__name__)
-
         # Inputs
         token_id_input = keras.Input(
             shape=(None,), dtype="int32", name="token_ids"
         )
         padding_mask = keras.Input(
             shape=(None,), dtype="int32", name="padding_mask"
         )
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,39 +11,39 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Test for DeBERTa backbone models."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
 class DebertaV3BackboneTest(TestCase):
     def setUp(self):
         self.backbone = DebertaV3Backbone(
             vocabulary_size=10,
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
             bucket_size=2,
         )
         self.batch_size = 8
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
 
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_valid_call_deberta(self):
@@ -55,20 +55,20 @@
     def test_token_embedding(self):
         output = self.backbone.token_embedding(self.input_batch["token_ids"])
         self.assertEqual(output.shape, (2, 5, 2))
 
     def test_variable_sequence_length_call_deberta(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "padding_mask": ops.ones((2, seq_length), dtype="int32"),
+                "token_ids": np.ones((2, seq_length), dtype="int32"),
+                "padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
             output = self.backbone(input_data)
             self.assertAllEqual(
-                tf.shape(output),
+                ops.shape(output),
                 [2, seq_length, self.backbone.hidden_dim],
             )
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
@@ -91,30 +91,29 @@
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
         self.assertAllClose(model_output, restored_output)
 
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
-@pytest.mark.tf_only
 class DebertaV3BackboneTPUTest(TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
             self.backbone = DebertaV3Backbone(
                 vocabulary_size=10,
                 num_layers=2,
                 num_heads=2,
                 hidden_dim=2,
                 intermediate_dim=4,
                 max_sequence_length=5,
                 bucket_size=2,
             )
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for DeBERTa classification model."""
 
 import io
 import os
 
+import numpy as np
 import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
@@ -29,15 +30,14 @@
 from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
 from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
 class DebertaV3ClassifierTest(TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
         sentencepiece.SentencePieceTrainer.train(
@@ -79,15 +79,15 @@
 
         self.raw_batch = [
             "the quick brown fox.",
             "the slow brown fox.",
         ]
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, ops.ones((2,)))
+            (self.raw_batch, np.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
     def test_classifier_predict(self):
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for DeBERTa preprocessor layer."""
 import io
-import os
 
-import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
     DebertaV3MaskedLMPreprocessor,
 )
@@ -49,15 +47,15 @@
             unk_piece="[UNK]",
             user_defined_symbols="[MASK]",
         )
         self.proto = bytes_io.getvalue()
         self.tokenizer = DebertaV3Tokenizer(proto=self.proto)
         self.preprocessor = DebertaV3MaskedLMPreprocessor(
             tokenizer=self.tokenizer,
-            # Simplify out testing by masking every available token.
+            # Simplify our testing by masking every available token.
             mask_selection_rate=1.0,
             mask_token_rate=1.0,
             random_token_rate=0.0,
             mask_selection_length=4,
             sequence_length=12,
         )
 
@@ -143,24 +141,7 @@
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs, y, sw = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        outputs = model(input_data)["token_ids"]
-        restored_outputs = restored_model(input_data)["token_ids"]
-        self.assertAllEqual(outputs, restored_outputs)
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
     DebertaV3MaskedLMPreprocessor,
 )
 from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
 class DebertaV3MaskedLMTest(TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round", "an eagle flew"]
         )
         sentencepiece.SentencePieceTrainer.train(
@@ -51,15 +50,19 @@
             eos_piece="[SEP]",
             unk_piece="[UNK]",
             user_defined_symbols="[MASK]",
         )
         proto = bytes_io.getvalue()
         self.preprocessor = DebertaV3MaskedLMPreprocessor(
             DebertaV3Tokenizer(proto=proto),
-            mask_selection_length=2,
+            # Simplify our testing by masking every available token.
+            mask_selection_rate=1.0,
+            mask_token_rate=1.0,
+            random_token_rate=0.0,
+            mask_selection_length=5,
             sequence_length=5,
         )
         self.backbone = DebertaV3Backbone(
             vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,161 +1,148 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for DeBERTa preprocessor layer."""
-import io
-import os
+"""Tests for RoBERTa masked language model preprocessor layer."""
 
-import pytest
-import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import (
-    DebertaV3Preprocessor,
+from keras_nlp.src.models.roberta.roberta_masked_lm_preprocessor import (
+    RobertaMaskedLMPreprocessor,
 )
-from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class DebertaV3PreprocessorTest(TestCase):
+class RobertaMaskedLMPreprocessorTest(TestCase):
     def setUp(self):
-        bytes_io = io.BytesIO()
-        vocab_data = tf.data.Dataset.from_tensor_slices(
-            ["the quick brown fox", "the earth is round"]
-        )
-        sentencepiece.SentencePieceTrainer.train(
-            sentence_iterator=vocab_data.as_numpy_iterator(),
-            model_writer=bytes_io,
-            vocab_size=12,
-            model_type="WORD",
-            pad_id=0,
-            bos_id=1,
-            eos_id=2,
-            unk_id=3,
-            pad_piece="[PAD]",
-            bos_piece="[CLS]",
-            eos_piece="[SEP]",
-            unk_piece="[UNK]",
-            user_defined_symbols="[MASK]",
-        )
-        self.proto = bytes_io.getvalue()
-
-        self.preprocessor = DebertaV3Preprocessor(
-            tokenizer=DebertaV3Tokenizer(proto=self.proto),
+        vocab = {
+            "<s>": 0,
+            "<pad>": 1,
+            "</s>": 2,
+            "Ġair": 3,
+            "plane": 4,
+            "Ġat": 5,
+            "port": 6,
+            "Ġkoh": 7,
+            "li": 8,
+            "Ġis": 9,
+            "Ġthe": 10,
+            "Ġbest": 11,
+            "<mask>": 12,
+        }
+
+        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
+        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
+        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
+        merges += ["pla ne"]
+
+        self.preprocessor = RobertaMaskedLMPreprocessor(
+            tokenizer=RobertaTokenizer(
+                vocabulary=vocab,
+                merges=merges,
+            ),
+            # Simplify our testing by masking every available token.
+            mask_selection_rate=1.0,
+            mask_token_rate=1.0,
+            random_token_rate=0.0,
+            mask_selection_length=5,
             sequence_length=12,
         )
 
-    def test_tokenize_strings(self):
-        input_data = "the quick brown fox"
-        output = self.preprocessor(input_data)
-        self.assertAllEqual(
-            output["token_ids"], [1, 5, 10, 6, 8, 2, 0, 0, 0, 0, 0, 0]
-        )
-        self.assertAllEqual(
-            output["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
-        )
+    def test_preprocess_strings(self):
+        input_data = " airplane at airport"
 
-    def test_tokenize_list_of_strings(self):
-        # We should handle a list of strings as as batch.
-        input_data = ["the quick brown fox"] * 4
-        output = self.preprocessor(input_data)
+        x, y, sw = self.preprocessor(input_data)
         self.assertAllEqual(
-            output["token_ids"], [[1, 5, 10, 6, 8, 2, 0, 0, 0, 0, 0, 0]] * 4
+            x["token_ids"], [0, 12, 12, 12, 12, 12, 2, 1, 1, 1, 1, 1]
         )
         self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
+            x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]
         )
+        self.assertAllEqual(x["mask_positions"], [1, 2, 3, 4, 5])
+        self.assertAllEqual(y, [3, 4, 5, 3, 6])
+        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0, 1.0])
 
-    def test_tokenize_labeled_batch(self):
-        x = tf.constant(["the quick brown fox"] * 4)
-        y = tf.constant([1] * 4)
-        sw = tf.constant([1.0] * 4)
-        x_out, y_out, sw_out = self.preprocessor(x, y, sw)
+    def test_preprocess_list_of_strings(self):
+        input_data = [" airplane at airport"] * 4
+
+        x, y, sw = self.preprocessor(input_data)
         self.assertAllEqual(
-            x_out["token_ids"], [[1, 5, 10, 6, 8, 2, 0, 0, 0, 0, 0, 0]] * 4
+            x["token_ids"], [[0, 12, 12, 12, 12, 12, 2, 1, 1, 1, 1, 1]] * 4
         )
         self.assertAllEqual(
-            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
+            x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]] * 4
         )
-        self.assertAllEqual(y_out, y)
-        self.assertAllEqual(sw_out, sw)
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4, 5]] * 4)
+        self.assertAllEqual(y, [[3, 4, 5, 3, 6]] * 4)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0, 1.0]] * 4)
 
-    def test_tokenize_labeled_dataset(self):
-        x = tf.constant(["the quick brown fox"] * 4)
-        y = tf.constant([1] * 4)
-        sw = tf.constant([1.0] * 4)
-        ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
+    def test_preprocess_dataset(self):
+        sentences = tf.constant([" airplane at airport"] * 4)
+        ds = tf.data.Dataset.from_tensor_slices(sentences)
         ds = ds.map(self.preprocessor)
-        x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
+        x, y, sw = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(
-            x_out["token_ids"], [[1, 5, 10, 6, 8, 2, 0, 0, 0, 0, 0, 0]] * 4
+            x["token_ids"], [[0, 12, 12, 12, 12, 12, 2, 1, 1, 1, 1, 1]] * 4
         )
         self.assertAllEqual(
-            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
+            x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]] * 4
         )
-        self.assertAllEqual(y_out, y)
-        self.assertAllEqual(sw_out, sw)
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4, 5]] * 4)
+        self.assertAllEqual(y, [[3, 4, 5, 3, 6]] * 4)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0, 1.0]] * 4)
+
+    def test_mask_multiple_sentences(self):
+        sentence_one = tf.constant(" airplane")
+        sentence_two = tf.constant(" kohli")
 
-    def test_tokenize_multiple_sentences(self):
-        sentence_one = tf.constant("the quick brown fox")
-        sentence_two = tf.constant("the earth")
-        output = self.preprocessor((sentence_one, sentence_two))
+        x, y, sw = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
-            output["token_ids"], [1, 5, 10, 6, 8, 2, 5, 7, 2, 0, 0, 0]
+            x["token_ids"], [0, 12, 12, 2, 2, 12, 12, 2, 1, 1, 1, 1]
         )
         self.assertAllEqual(
-            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]
+            x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0]
         )
+        self.assertAllEqual(x["mask_positions"], [1, 2, 5, 6, 0])
+        self.assertAllEqual(y, [3, 4, 7, 8, 0])
+        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0, 0.0])
 
-    def test_tokenize_multiple_batched_sentences(self):
-        sentence_one = tf.constant(["the quick brown fox"] * 4)
-        sentence_two = tf.constant(["the earth"] * 4)
-        # The first tuple or list is always interpreted as an enumeration of
-        # separate sequences to concatenate.
-        output = self.preprocessor((sentence_one, sentence_two))
+    def test_no_masking_zero_rate(self):
+        no_mask_preprocessor = RobertaMaskedLMPreprocessor(
+            self.preprocessor.tokenizer,
+            mask_selection_rate=0.0,
+            mask_selection_length=5,
+            sequence_length=12,
+        )
+        input_data = " airplane at airport"
+
+        x, y, sw = no_mask_preprocessor(input_data)
         self.assertAllEqual(
-            output["token_ids"], [[1, 5, 10, 6, 8, 2, 5, 7, 2, 0, 0, 0]] * 4
+            x["token_ids"], [0, 3, 4, 5, 3, 6, 2, 1, 1, 1, 1, 1]
         )
         self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]] * 4
+            x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]
         )
-
-    def test_errors_for_2d_list_input(self):
-        ambiguous_input = [["one", "two"], ["three", "four"]]
-        with self.assertRaises(ValueError):
-            self.preprocessor(ambiguous_input)
+        self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0, 0])
+        self.assertAllEqual(y, [0, 0, 0, 0, 0])
+        self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0, 0.0])
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     DebertaV3Preprocessor,
 )
 from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
 @pytest.mark.large
-@pytest.mark.tf_only
 class DebertaV3PresetSmokeTest(TestCase):
     """
     A smoke test for DeBERTa presets we run continuously.
 
     This only tests the smallest weights we have available. Run with:
     `pytest keras_nlp/models/deberta/deberta_presets_test.py --run_large`
     """
@@ -130,15 +129,14 @@
     def test_unknown_preset_error(self, cls, kwargs):
         # Not a preset name
         with self.assertRaises(ValueError):
             cls.from_preset("deberta_v3_extra_small_en_clowntown", **kwargs)
 
 
 @pytest.mark.extra_large
-@pytest.mark.tf_only
 class DebertaV3PresetFullTest(TestCase):
     """
     Test the full enumeration of our preset.
 
     This tests every DeBERTa preset and is only run manually.
     Run with:
     `pytest keras_nlp/models/deberta/deberta_presets_test.py --run_extra_large`
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_tokenizer_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,115 +8,85 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for DeBERTa tokenizer."""
+"""Tests for FNet tokenizer."""
 import io
-import os
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class DebertaV3TokenizerTest(TestCase):
+@pytest.mark.tf_only
+class FNetTokenizerTest(TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
-            vocab_size=10,
+            vocab_size=12,
             model_type="WORD",
-            pad_id=0,
-            bos_id=1,
-            eos_id=2,
-            unk_id=3,
-            pad_piece="[PAD]",
+            pad_id=3,
+            unk_id=0,
+            bos_id=4,
+            eos_id=5,
+            pad_piece="<pad>",
+            unk_piece="<unk>",
             bos_piece="[CLS]",
             eos_piece="[SEP]",
-            unk_piece="[UNK]",
+            user_defined_symbols="[MASK]",
         )
         self.proto = bytes_io.getvalue()
 
-        self.tokenizer = DebertaV3Tokenizer(proto=self.proto)
+        self.tokenizer = FNetTokenizer(proto=self.proto)
 
     def test_tokenize(self):
         input_data = "the quick brown fox"
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [4, 9, 5, 7])
+        self.assertAllEqual(output, [2, 10, 6, 8])
 
     def test_tokenize_batch(self):
         input_data = ["the quick brown fox", "the earth is round"]
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [[4, 9, 5, 7], [4, 6, 8, 3]])
+        self.assertAllEqual(output, [[2, 10, 6, 8], [2, 7, 9, 11]])
 
     def test_detokenize(self):
-        input_data = [[4, 9, 5, 7]]
-        output = self.tokenizer.detokenize(input_data)
-        self.assertEqual(output, ["the quick brown fox"])
-
-    def test_detokenize_mask_token(self):
-        input_data = [[4, 9, 5, 7, self.tokenizer.mask_token_id]]
+        input_data = [[2, 10, 6, 8]]
         output = self.tokenizer.detokenize(input_data)
         self.assertEqual(output, ["the quick brown fox"])
 
     def test_vocabulary_size(self):
-        self.assertEqual(self.tokenizer.vocabulary_size(), 11)
-
-    def test_get_vocabulary_mask_token(self):
-        self.assertEqual(self.tokenizer.get_vocabulary()[10], "[MASK]")
-
-    def test_id_to_token_mask_token(self):
-        self.assertEqual(self.tokenizer.id_to_token(10), "[MASK]")
-
-    def test_token_to_id_mask_token(self):
-        self.assertEqual(self.tokenizer.token_to_id("[MASK]"), 10)
+        tokenizer = FNetTokenizer(proto=self.proto)
+        self.assertEqual(tokenizer.vocabulary_size(), 12)
 
     def test_errors_missing_special_tokens(self):
         bytes_io = io.BytesIO()
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=iter(["abc"]),
             model_writer=bytes_io,
             vocab_size=5,
             pad_id=-1,
             eos_id=-1,
             bos_id=-1,
         )
         with self.assertRaises(ValueError):
-            DebertaV3Tokenizer(proto=bytes_io.getvalue())
+            FNetTokenizer(proto=bytes_io.getvalue())
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.tokenizer)
         new_tokenizer = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_tokenizer.get_config(),
             self.tokenizer.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Disentangled self-attention layer."""
 
 import math
 
-import tensorflow as tf
-
 from keras_nlp.src.backend import keras
+from keras_nlp.src.backend import ops
 from keras_nlp.src.utils.keras_utils import clone_initializer
 
 
 class DisentangledSelfAttention(keras.layers.Layer):
     """DisentangledSelfAttention layer.
 
     This is an implementation of disentangled self-attention as described in the
@@ -146,17 +145,17 @@
         This implementation is the similar to the one present in
         `keras.layers.MultiHeadAttention`.
         """
 
         if attention_mask is not None:
             mask_expansion_axis = -3
             for _ in range(
-                attention_scores.shape.rank - attention_mask.shape.rank
+                len(attention_scores.shape) - len(attention_mask.shape)
             ):
-                attention_mask = tf.expand_dims(
+                attention_mask = ops.expand_dims(
                     attention_mask, axis=mask_expansion_axis
                 )
         return self._softmax(attention_scores, attention_mask)
 
     def _compute_attention(
         self,
         query,
@@ -169,20 +168,20 @@
         """Computes the attention score and returns the attended outputs.
 
         This function computes vanilla MHA score, and relative attention scores
         (p2c and c2p). It then sums them up to get the final attention score,
         which is used to compute the attended outputs.
         """
 
-        attention_scores = tf.einsum(
+        attention_scores = ops.einsum(
             "aecd,abcd->acbe",
             key,
             query,
         )
-        attention_scores = tf.multiply(attention_scores, self.scale_factor)
+        attention_scores = ops.multiply(attention_scores, self.scale_factor)
 
         rel_embeddings = self._position_dropout_layer(
             rel_embeddings,
             training=training,
         )
 
         rel_attn_scores = self._compute_disentangled_attention(
@@ -196,134 +195,132 @@
 
         attention_scores = self._masked_softmax(
             attention_scores, attention_mask
         )
         attention_scores = self._attn_dropout_layer(
             attention_scores, training=training
         )
-        attention_output = tf.einsum("acbe,aecd->abcd", attention_scores, value)
+        attention_output = ops.einsum(
+            "acbe,aecd->abcd", attention_scores, value
+        )
 
         return attention_output, attention_scores
 
     def _make_log_bucket_position(self, rel_pos):
         dtype = rel_pos.dtype
-        sign = tf.math.sign(rel_pos)
+        sign = ops.sign(rel_pos)
         mid = self.bucket_size // 2
-        mid = tf.cast(mid, dtype=dtype)
+        mid = ops.cast(mid, dtype=dtype)
 
         # If `rel_pos[i][j]` is out of bounds, assign value `mid`.
-        abs_pos = tf.where(
+        abs_pos = ops.where(
             condition=(rel_pos < mid) & (rel_pos > -mid),
-            x=mid - 1,
-            y=tf.math.abs(rel_pos),
+            x1=mid - 1,
+            x2=ops.abs(rel_pos),
         )
 
         def _get_log_pos(abs_pos, mid):
-            numerator = tf.math.log(abs_pos / mid)
-            numerator = numerator * tf.cast(mid - 1, dtype=numerator.dtype)
-            denominator = tf.math.log((self.max_position_embeddings - 1) / mid)
-            val = tf.math.ceil(numerator / denominator)
-            val = tf.cast(val, dtype=mid.dtype)
+            numerator = ops.log(abs_pos / mid)
+            numerator = numerator * ops.cast(mid - 1, dtype=numerator.dtype)
+            denominator = ops.log((self.max_position_embeddings - 1) / mid)
+            val = ops.ceil(numerator / denominator)
+            val = ops.cast(val, dtype=mid.dtype)
             val = val + mid
             return val
 
         log_pos = _get_log_pos(abs_pos, mid)
 
-        bucket_pos = tf.where(
+        bucket_pos = ops.where(
             condition=abs_pos <= mid,
-            x=rel_pos,
-            y=log_pos * sign,
+            x1=rel_pos,
+            x2=log_pos * sign,
         )
-        bucket_pos = tf.cast(bucket_pos, dtype="int64")
+        bucket_pos = ops.cast(bucket_pos, dtype="int64")
 
         return bucket_pos
 
     def _get_rel_pos(self, num_positions):
-        ids = tf.range(num_positions, dtype="int64")
-        query_ids = ids[:, tf.newaxis]
-        key_ids = ids[tf.newaxis, :]
-        key_ids = tf.repeat(key_ids, repeats=num_positions, axis=0)
+        ids = ops.arange(num_positions, dtype="int64")
+        query_ids = ops.expand_dims(ids, axis=-1)
+        key_ids = ops.expand_dims(ids, axis=0)
+        key_ids = ops.repeat(key_ids, repeats=num_positions, axis=0)
 
         rel_pos = query_ids - key_ids
         rel_pos = self._make_log_bucket_position(rel_pos)
 
-        rel_pos = rel_pos[tf.newaxis, tf.newaxis, :, :]
+        rel_pos = ops.expand_dims(ops.expand_dims(rel_pos, axis=0), axis=0)
         return rel_pos
 
     def _compute_disentangled_attention(
         self,
         query,
         key,
         rel_embeddings,
     ):
         """Computes relative attention scores (p2c and c2p)."""
 
-        batch_size = tf.shape(query)[0]
-        num_positions = tf.shape(query)[1]
+        batch_size = ops.shape(query)[0]
+        num_positions = ops.shape(query)[1]
 
         rel_pos = self._get_rel_pos(num_positions)
 
         rel_attn_span = self.bucket_size
         score = 0
 
         pos_query = self._query_dense(rel_embeddings)
         pos_key = self._key_dense(rel_embeddings)
 
         # c2p
-        c2p_attn_scores = tf.einsum(
+        c2p_attn_scores = ops.einsum(
             "aecd,abcd->acbe",
             pos_key,
             query,
         )
-        c2p_pos = tf.clip_by_value(
-            rel_pos + rel_attn_span, 0, rel_attn_span * 2 - 1
-        )
-        c2p_pos = tf.broadcast_to(
+        c2p_pos = ops.clip(rel_pos + rel_attn_span, 0, rel_attn_span * 2 - 1)
+        c2p_pos = ops.broadcast_to(
             c2p_pos,
             shape=(
                 batch_size,
                 self.num_heads,
                 num_positions,
                 num_positions,
             ),
         )
 
-        c2p_attn_scores = tf.gather(
+        c2p_attn_scores = ops.take_along_axis(
             c2p_attn_scores,
             indices=c2p_pos,
-            batch_dims=3,
+            axis=3,
         )
-        c2p_attn_scores = tf.multiply(c2p_attn_scores, self.scale_factor)
+        c2p_attn_scores = ops.multiply(c2p_attn_scores, self.scale_factor)
         score += c2p_attn_scores
 
         # p2c
-        p2c_attn_scores = tf.einsum(
+        p2c_attn_scores = ops.einsum(
             "aecd,abcd->acbe",
             pos_query,
             key,
         )
-        p2c_pos = tf.clip_by_value(
-            -rel_pos + rel_attn_span, 0, rel_attn_span * 2 - 1
-        )
-        p2c_pos = tf.broadcast_to(
+        p2c_pos = ops.clip(-rel_pos + rel_attn_span, 0, rel_attn_span * 2 - 1)
+        p2c_pos = ops.broadcast_to(
             p2c_pos,
             shape=(
                 batch_size,
                 self.num_heads,
                 num_positions,
                 num_positions,
             ),
         )
-        p2c_attn_scores = tf.gather(
+        p2c_attn_scores = ops.take_along_axis(
             p2c_attn_scores,
             indices=p2c_pos,
-            batch_dims=3,
+            axis=3,
         )
-        p2c_attn_scores = tf.transpose(p2c_attn_scores, [0, 1, 3, 2])
-        p2c_attn_scores = tf.multiply(p2c_attn_scores, self.scale_factor)
+        p2c_attn_scores = ops.transpose(p2c_attn_scores, [0, 1, 3, 2])
+        p2c_attn_scores = ops.multiply(p2c_attn_scores, self.scale_factor)
         score += p2c_attn_scores
 
         return score
 
     def call(
         self,
         inputs,
@@ -344,19 +341,19 @@
             value=value,
             rel_embeddings=rel_embeddings,
             attention_mask=attention_mask,
             training=training,
         )
 
         # Reshape `attention_output` to `(batch_size, sequence_length, hidden_dim)`.
-        attention_output = tf.reshape(
+        attention_output = ops.reshape(
             attention_output,
             [
-                tf.shape(attention_output)[0],
-                tf.shape(attention_output)[1],
+                ops.shape(attention_output)[0],
+                ops.shape(attention_output)[1],
                 self.hidden_dim,
             ],
         )
         attention_output = self._output_dense(attention_output)
 
         if return_attention_scores:
             return attention_output, attention_scores
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/deberta_v3/relative_embedding.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/deberta_v3/relative_embedding.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Relative embedding layer."""
 
-import tensorflow as tf
-
 from keras_nlp.src.backend import keras
+from keras_nlp.src.backend import ops
 
 
 class RelativeEmbedding(keras.layers.Layer):
     """Relative embedding layer.
 
     This is an implementation of relative embedding as described in the
     paper ["DeBERTaV3: Improving DeBERTa using ELECTRA-Style Pre-Training with Gradient-Disentangled Embedding Sharing"](https://arxiv.org/abs/2111.09543).
@@ -60,22 +59,24 @@
             name="rel_embedding",
         )
         self.layer_norm = keras.layers.LayerNormalization(
             epsilon=layer_norm_epsilon, name="rel_embeddings_layer_norm"
         )
 
     def call(self, inputs):
-        batch_size = tf.shape(inputs)[0]
+        batch_size = ops.shape(inputs)[0]
 
-        rel_embeddings = self.rel_embeddings[tf.newaxis, :]
+        rel_embeddings = ops.expand_dims(
+            ops.convert_to_tensor(self.rel_embeddings), axis=0
+        )
         rel_embeddings = self.layer_norm(rel_embeddings)
 
         # Repeat `rel_embeddings` along axis = 0 `batch_size` times. The
         # resultant shape is `(batch_size, bucket_size * 2, hidden_dim)`.
-        rel_embeddings = tf.repeat(rel_embeddings, repeats=batch_size, axis=0)
+        rel_embeddings = ops.repeat(rel_embeddings, repeats=batch_size, axis=0)
 
         return rel_embeddings
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_backbone_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,61 +7,63 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for DistilBERT backbone models."""
+"""Test for BERT backbone models."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
-from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
+from keras_nlp.src.models.bert.bert_backbone import BertBackbone
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class DistilBertTest(TestCase):
+class BertBackboneTest(TestCase):
     def setUp(self):
-        self.backbone = DistilBertBackbone(
+        self.backbone = BertBackbone(
             vocabulary_size=10,
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
-            name="encoder",
         )
-
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "segment_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
-
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
-    def test_valid_call_distilbert(self):
+    def test_valid_call_bert(self):
         self.backbone(self.input_batch)
 
     def test_token_embedding(self):
         output = self.backbone.token_embedding(self.input_batch["token_ids"])
         self.assertEqual(output.shape, (2, 5, 2))
 
-    def test_variable_sequence_length_call_distilbert(self):
+    def test_name(self):
+        # Check default name passed through
+        self.assertRegexpMatches(self.backbone.name, "bert_backbone")
+
+    def test_variable_sequence_length_call_bert(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "mask_positions": ops.ones((2, seq_length), dtype="int32"),
-                "padding_mask": ops.ones((2, seq_length), dtype="int32"),
+                "token_ids": np.ones((2, seq_length), dtype="int32"),
+                "segment_ids": np.ones((2, seq_length), dtype="int32"),
+                "padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
             self.backbone(input_data)
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
@@ -75,37 +77,38 @@
     def test_saved_model(self):
         model_output = self.backbone(self.input_batch)
         path = os.path.join(self.get_temp_dir(), "model.keras")
         self.backbone.save(path, save_format="keras_v3")
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, DistilBertBackbone)
+        self.assertIsInstance(restored_model, BertBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
         self.assertAllClose(model_output, restored_output)
 
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
-class DistilBertTPUTest(TestCase):
+class BertBackboneTPUTest(TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
-            self.backbone = DistilBertBackbone(
+            self.backbone = BertBackbone(
                 vocabulary_size=1000,
                 num_layers=2,
                 num_heads=2,
                 hidden_dim=64,
                 intermediate_dim=128,
                 max_sequence_length=128,
             )
         self.input_batch = {
-            "token_ids": ops.ones((8, 128), dtype="int32"),
-            "padding_mask": ops.ones((8, 128), dtype="int32"),
+            "token_ids": np.ones((8, 128), dtype="int32"),
+            "segment_ids": np.ones((8, 128), dtype="int32"),
+            "padding_mask": np.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for DistilBERT classification model."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 from keras_nlp.src.models.distil_bert.distil_bert_classifier import (
@@ -62,15 +63,15 @@
 
         self.raw_batch = [
             "the quick brown fox.",
             "the slow brown fox.",
         ]
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, ops.ones((2,)))
+            (self.raw_batch, np.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
     def test_classifier_predict(self):
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for DistilBERT masked language model preprocessor layer."""
-import os
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.distil_bert.distil_bert_masked_lm_preprocessor import (
     DistilBertMaskedLMPreprocessor,
 )
 from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
@@ -34,15 +32,15 @@
         self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
         self.vocab += ["the", "quick", "brown", "fox"]
 
         self.preprocessor = DistilBertMaskedLMPreprocessor(
             tokenizer=DistilBertTokenizer(
                 vocabulary=self.vocab,
             ),
-            # Simplify out testing by masking every available token.
+            # Simplify our testing by masking every available token.
             mask_selection_rate=1.0,
             mask_token_rate=1.0,
             random_token_rate=0.0,
             mask_selection_length=5,
             sequence_length=8,
         )
 
@@ -108,24 +106,7 @@
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant([" THE QUICK BROWN FOX."])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs, y, sw = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        outputs = model(input_data)["token_ids"]
-        restored_outputs = restored_model(input_data)["token_ids"]
-        self.assertAllEqual(outputs, restored_outputs)
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,20 @@
 class DistilBertMaskedLMTest(TestCase):
     def setUp(self):
         # Setup model.
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["the", "quick", "brown", "fox", "."]
         self.preprocessor = DistilBertMaskedLMPreprocessor(
             DistilBertTokenizer(vocabulary=self.vocab),
+            # Simplify our testing by masking every available token.
+            mask_selection_rate=1.0,
+            mask_token_rate=1.0,
+            random_token_rate=0.0,
+            mask_selection_length=5,
             sequence_length=5,
-            mask_selection_length=2,
         )
         self.backbone = DistilBertBackbone(
             vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             num_heads=2,
             hidden_dim=4,
             intermediate_dim=4,
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_preprocessor_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,97 +7,105 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for DistilBERT preprocessor layer."""
+"""Tests for BERT preprocessor layer."""
 
-import os
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
-    DistilBertPreprocessor,
-)
-from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
-    DistilBertTokenizer,
-)
+from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
+from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class DistilBertPreprocessorTest(TestCase):
+class BertPreprocessorTest(TestCase):
     def setUp(self):
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
         self.vocab += ["the", "quick", "brown", "fox"]
-        self.preprocessor = DistilBertPreprocessor(
-            DistilBertTokenizer(vocabulary=self.vocab),
+        self.preprocessor = BertPreprocessor(
+            BertTokenizer(vocabulary=self.vocab),
             sequence_length=8,
         )
 
     def test_tokenize_strings(self):
         input_data = "THE QUICK BROWN FOX."
         output = self.preprocessor(input_data)
         self.assertAllEqual(output["token_ids"], [2, 5, 6, 7, 8, 1, 3, 0])
+        self.assertAllEqual(output["segment_ids"], [0, 0, 0, 0, 0, 0, 0, 0])
         self.assertAllEqual(output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
 
     def test_tokenize_list_of_strings(self):
         # We should handle a list of strings as as batch.
         input_data = ["THE QUICK BROWN FOX."] * 4
         output = self.preprocessor(input_data)
         self.assertAllEqual(output["token_ids"], [[2, 5, 6, 7, 8, 1, 3, 0]] * 4)
         self.assertAllEqual(
+            output["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(
             output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4
         )
 
     def test_tokenize_labeled_batch(self):
         x = tf.constant(["THE QUICK BROWN FOX."] * 4)
         y = tf.constant([1] * 4)
         sw = tf.constant([1.0] * 4)
         x_out, y_out, sw_out = self.preprocessor(x, y, sw)
         self.assertAllEqual(x_out["token_ids"], [[2, 5, 6, 7, 8, 1, 3, 0]] * 4)
         self.assertAllEqual(
+            x_out["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(
             x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4
         )
         self.assertAllEqual(y_out, y)
         self.assertAllEqual(sw_out, sw)
 
     def test_tokenize_labeled_dataset(self):
         x = tf.constant(["THE QUICK BROWN FOX."] * 4)
         y = tf.constant([1] * 4)
         sw = tf.constant([1.0] * 4)
         ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
         ds = ds.map(self.preprocessor)
         x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(x_out["token_ids"], [[2, 5, 6, 7, 8, 1, 3, 0]] * 4)
         self.assertAllEqual(
+            x_out["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(
             x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4
         )
         self.assertAllEqual(y_out, y)
         self.assertAllEqual(sw_out, sw)
 
     def test_tokenize_multiple_sentences(self):
         sentence_one = tf.constant("THE QUICK")
         sentence_two = tf.constant("BROWN FOX.")
         output = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(output["token_ids"], [2, 5, 6, 3, 7, 8, 1, 3])
+        self.assertAllEqual(output["segment_ids"], [0, 0, 0, 0, 1, 1, 1, 1])
         self.assertAllEqual(output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1])
 
     def test_tokenize_multiple_batched_sentences(self):
         sentence_one = tf.constant(["THE QUICK"] * 4)
         sentence_two = tf.constant(["BROWN FOX."] * 4)
         # The first tuple or list is always interpreted as an enumeration of
         # separate sequences to concatenate.
         output = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(output["token_ids"], [[2, 5, 6, 3, 7, 8, 1, 3]] * 4)
         self.assertAllEqual(
+            output["segment_ids"], [[0, 0, 0, 0, 1, 1, 1, 1]] * 4
+        )
+        self.assertAllEqual(
             output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1]] * 4
         )
 
     def test_errors_for_2d_list_input(self):
         ambiguous_input = [["one", "two"], ["three", "four"]]
         with self.assertRaises(ValueError):
             self.preprocessor(ambiguous_input)
@@ -106,22 +114,7 @@
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["THE QUICK BROWN FOX."])
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for DistilBERT tokenizer."""
 
-import os
-
-import pytest
-import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
 from keras_nlp.src.tests.test_case import TestCase
 
@@ -64,23 +60,7 @@
         config = keras.saving.serialize_keras_object(self.tokenizer)
         new_tokenizer = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_tokenizer.get_config(),
             self.tokenizer.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["THE QUICK BROWN FOX."])
-        tokenizer = DistilBertTokenizer(vocabulary=self.vocab)
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_backbone_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,104 +7,123 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for FNet backbone model."""
+"""Test for OPT backbone models."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
-from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
-class FNetBackboneTest(TestCase):
+class OPTBackboneTest(TestCase):
     def setUp(self):
-        self.backbone = FNetBackbone(
+        self.backbone = OPTBackbone(
             vocabulary_size=10,
             num_layers=2,
+            num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
-            num_segments=4,
         )
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "segment_ids": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
 
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
-    def test_valid_call_f_net(self):
+    def test_valid_call_opt(self):
         self.backbone(self.input_batch)
 
+    def test_token_embedding(self):
+        output = self.backbone.token_embedding(self.input_batch["token_ids"])
+        self.assertEqual(output.shape, (2, 5, 2))
+
+    def test_name(self):
         # Check default name passed through
-        self.assertRegexpMatches(self.backbone.name, "f_net_backbone")
+        self.assertRegexpMatches(self.backbone.name, "opt_backbone")
 
-    def test_variable_sequence_length_call_f_net(self):
+    def test_variable_sequence_length_call_opt(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "segment_ids": ops.ones((2, seq_length), dtype="int32"),
+                "token_ids": np.ones((2, seq_length), dtype="int32"),
+                "padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
             self.backbone(input_data)
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
     def test_serialization(self):
         new_backbone = keras.saving.deserialize_keras_object(
             keras.saving.serialize_keras_object(self.backbone)
         )
         self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
-    @pytest.mark.large
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self):
         model_output = self.backbone(self.input_batch)
         path = os.path.join(self.get_temp_dir(), "model.keras")
         self.backbone.save(path, save_format="keras_v3")
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, FNetBackbone)
+        self.assertIsInstance(restored_model, OPTBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
-        self.assertAllClose(
-            model_output["pooled_output"], restored_output["pooled_output"]
-        )
+        self.assertAllClose(model_output, restored_output)
+
+    def test_create_layout_map(self):
+        mesh = tf.experimental.dtensor.create_mesh([("batch", 1), ("model", 1)])
+        with OPTBackbone.create_layout_map(mesh).scope():
+            OPTBackbone(
+                vocabulary_size=10,
+                num_layers=2,
+                num_heads=2,
+                hidden_dim=2,
+                intermediate_dim=4,
+                max_sequence_length=5,
+            )
+        # Using DTensor enables the mlir bridge as a side effect. Eventually
+        # this will be default, but for now we have compile errors with the
+        # bridge elsewhere and must disable. See
+        # https://github.com/keras-team/keras-nlp/issues/1001
+        tf.config.experimental.disable_mlir_bridge()
 
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
-class FNetBackboneTPUTest(TestCase):
+class OPTBackboneTPUTest(TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
-            self.backbone = FNetBackbone(
-                vocabulary_size=100,
+            self.backbone = OPTBackbone(
+                vocabulary_size=1000,
                 num_layers=2,
-                hidden_dim=16,
-                intermediate_dim=32,
+                num_heads=2,
+                hidden_dim=32,
+                intermediate_dim=128,
                 max_sequence_length=128,
-                num_segments=4,
             )
         self.input_batch = {
-            "token_ids": ops.ones((8, 128), dtype="int32"),
-            "segment_ids": ops.ones((8, 128), dtype="int32"),
+            "token_ids": np.ones((8, 128), dtype="int32"),
+            "padding_mask": np.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_classifier.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_classifier_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_classifier_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for FNet classification model."""
 
 import io
 import os
 
+import numpy as np
 import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
 from keras_nlp.src.models.f_net.f_net_classifier import FNetClassifier
 from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
 class FNetClassifierTest(TestCase):
     def setUp(self):
         # Setup Model
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
@@ -78,15 +78,15 @@
         # Setup data.
         self.raw_batch = [
             "the quick brown fox.",
             "the slow brown fox.",
         ]
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, ops.ones((2,)))
+            (self.raw_batch, np.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
     def test_classifier_predict(self):
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,142 +7,129 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import io
-import os
+"""Tests for BERT masked language model preprocessor layer."""
+
 
-import pytest
-import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import (
-    FNetMaskedLMPreprocessor,
+from keras_nlp.src.models.bert.bert_masked_lm_preprocessor import (
+    BertMaskedLMPreprocessor,
 )
-from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class FNetMaskedLMPreprocessorTest(TestCase):
+class BertMaskedLMPreprocessorTest(TestCase):
     def setUp(self):
-        bytes_io = io.BytesIO()
-        vocab_data = tf.data.Dataset.from_tensor_slices(
-            ["the quick brown fox", "the earth is round"]
-        )
-        sentencepiece.SentencePieceTrainer.train(
-            sentence_iterator=vocab_data.as_numpy_iterator(),
-            model_writer=bytes_io,
-            vocab_size=12,
-            model_type="WORD",
-            pad_id=0,
-            bos_id=1,
-            eos_id=2,
-            unk_id=3,
-            pad_piece="<pad>",
-            unk_piece="<unk>",
-            bos_piece="[CLS]",
-            eos_piece="[SEP]",
-            user_defined_symbols="[MASK]",
-        )
-        self.proto = bytes_io.getvalue()
-
-        self.preprocessor = FNetMaskedLMPreprocessor(
-            tokenizer=FNetTokenizer(proto=self.proto),
+        self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
+        self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
+        self.vocab += ["the", "quick", "brown", "fox"]
+
+        tokenizer = BertTokenizer(vocabulary=self.vocab)
+
+        self.preprocessor = BertMaskedLMPreprocessor(
+            tokenizer=tokenizer,
+            # Simplify our testing by masking every available token.
             mask_selection_rate=1.0,
             mask_token_rate=1.0,
             random_token_rate=0.0,
             mask_selection_length=4,
             sequence_length=12,
         )
 
     def test_preprocess_strings(self):
         input_data = "the quick brown fox"
 
         x, y, sw = self.preprocessor(input_data)
         self.assertAllEqual(
-            x["token_ids"], [1, 4, 4, 4, 4, 2, 0, 0, 0, 0, 0, 0]
+            x["token_ids"], [2, 4, 4, 4, 4, 3, 0, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(
+            x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(
+            x["segment_ids"], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
         )
         self.assertAllEqual(x["mask_positions"], [1, 2, 3, 4])
-        self.assertAllEqual(y, [5, 10, 6, 8])
+        self.assertAllEqual(y, [9, 10, 11, 12])
         self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0])
 
     def test_preprocess_list_of_strings(self):
         input_data = ["the quick brown fox"] * 4
 
         x, y, sw = self.preprocessor(input_data)
         self.assertAllEqual(
-            x["token_ids"], [[1, 4, 4, 4, 4, 2, 0, 0, 0, 0, 0, 0]] * 4
+            x["token_ids"], [[2, 4, 4, 4, 4, 3, 0, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(
+            x["padding_mask"],
+            [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4,
         )
         self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4]] * 4)
-        self.assertAllEqual(y, [[5, 10, 6, 8]] * 4)
+        self.assertAllEqual(y, [[9, 10, 11, 12]] * 4)
         self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0]] * 4)
 
     def test_preprocess_dataset(self):
         sentences = tf.constant(["the quick brown fox"] * 4)
         ds = tf.data.Dataset.from_tensor_slices(sentences)
         ds = ds.map(self.preprocessor)
         x, y, sw = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(
-            x["token_ids"], [[1, 4, 4, 4, 4, 2, 0, 0, 0, 0, 0, 0]] * 4
+            x["token_ids"], [[2, 4, 4, 4, 4, 3, 0, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(
+            x["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4]] * 4)
-        self.assertAllEqual(y, [[5, 10, 6, 8]] * 4)
+        self.assertAllEqual(y, [[9, 10, 11, 12]] * 4)
         self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0]] * 4)
 
     def test_mask_multiple_sentences(self):
         sentence_one = tf.constant("the quick")
         sentence_two = tf.constant("brown fox")
 
         x, y, sw = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
-            x["token_ids"], [1, 4, 4, 2, 4, 4, 2, 0, 0, 0, 0, 0]
+            x["token_ids"], [2, 4, 4, 3, 4, 4, 3, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(
+            x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]
         )
         self.assertAllEqual(x["mask_positions"], [1, 2, 4, 5])
-        self.assertAllEqual(y, [5, 10, 6, 8])
+        self.assertAllEqual(y, [9, 10, 11, 12])
         self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0])
 
     def test_no_masking_zero_rate(self):
-        no_mask_preprocessor = FNetMaskedLMPreprocessor(
+        no_mask_preprocessor = BertMaskedLMPreprocessor(
             self.preprocessor.tokenizer,
             mask_selection_rate=0.0,
             mask_selection_length=4,
             sequence_length=12,
         )
         input_data = "the quick brown fox"
 
         x, y, sw = no_mask_preprocessor(input_data)
         self.assertAllEqual(
-            x["token_ids"], [1, 5, 10, 6, 8, 2, 0, 0, 0, 0, 0, 0]
+            x["token_ids"], [2, 9, 10, 11, 12, 3, 0, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(
+            x["padding_mask"],
+            [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0],
         )
         self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0])
         self.assertAllEqual(y, [0, 0, 0, 0])
         self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0])
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs, y, sw = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        outputs = model(input_data)["token_ids"]
-        restored_outputs = restored_model(input_data)["token_ids"]
-        self.assertAllEqual(outputs, restored_outputs)
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import (
     FNetMaskedLMPreprocessor,
 )
 from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
 class FNetMaskedLMTest(TestCase):
     def setUp(self):
         # Setup Model.
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the slow brown fox"]
         )
@@ -50,16 +49,20 @@
             bos_piece="[CLS]",
             eos_piece="[SEP]",
             user_defined_symbols="[MASK]",
         )
         self.proto = bytes_io.getvalue()
         self.preprocessor = FNetMaskedLMPreprocessor(
             FNetTokenizer(proto=self.proto),
+            # Simplify our testing by masking every available token.
+            mask_selection_rate=1.0,
+            mask_token_rate=1.0,
+            random_token_rate=0.0,
+            mask_selection_length=5,
             sequence_length=5,
-            mask_selection_length=2,
         )
         self.backbone = FNetBackbone(
             vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=self.preprocessor.packer.sequence_length,
@@ -78,25 +81,25 @@
             self.raw_batch
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.masked_lm(self.preprocessed_batch)
 
-    def test_classifier_predict(self):
+    def test_predict(self):
         # self.masked_lm.predict(self.raw_batch)
         self.masked_lm.preprocessor = None
         self.masked_lm.predict(self.preprocessed_batch)
 
-    def test_classifier_fit(self):
+    def test_fit(self):
         self.masked_lm.fit(self.raw_dataset)
         self.masked_lm.preprocessor = None
         self.masked_lm.fit(self.preprocessed_dataset)
 
-    def test_classifier_fit_no_xla(self):
+    def test_fit_no_xla(self):
         self.masked_lm.preprocessor = None
         self.masked_lm.compile(
             loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False),
             jit_compile=False,
         )
         self.masked_lm.fit(self.preprocessed_dataset)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_preprocessor_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for FNet preprocessor layer."""
 import io
-import os
 
-import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 from keras_nlp.src.tests.test_case import TestCase
@@ -143,22 +141,7 @@
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_presets_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from keras_nlp.src.models.f_net.f_net_classifier import FNetClassifier
 from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
 @pytest.mark.large
-@pytest.mark.tf_only
 class FNetPresetSmokeTest(TestCase):
     """
     A smoke test for FNet presets we run continuously.
 
     This only tests the smallest weights we have available. Run with:
     `pytest keras_nlp/models/f_net/f_net_presets_test.py --run_large`
     """
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/f_net/f_net_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/albert/albert_tokenizer_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,104 +8,83 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for FNet tokenizer."""
+"""Tests for ALBERT tokenizer."""
 import io
-import os
 
-import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
-class FNetTokenizerTest(TestCase):
+class AlbertTokenizerTest(TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
             vocab_size=12,
             model_type="WORD",
-            pad_id=3,
-            unk_id=0,
-            bos_id=4,
-            eos_id=5,
+            pad_id=0,
+            unk_id=1,
+            bos_id=2,
+            eos_id=3,
             pad_piece="<pad>",
             unk_piece="<unk>",
             bos_piece="[CLS]",
             eos_piece="[SEP]",
             user_defined_symbols="[MASK]",
         )
         self.proto = bytes_io.getvalue()
 
-        self.tokenizer = FNetTokenizer(proto=self.proto)
+        self.tokenizer = AlbertTokenizer(proto=self.proto)
 
     def test_tokenize(self):
         input_data = "the quick brown fox"
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [2, 10, 6, 8])
+        self.assertAllEqual(output, [5, 10, 6, 8])
 
     def test_tokenize_batch(self):
         input_data = ["the quick brown fox", "the earth is round"]
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [[2, 10, 6, 8], [2, 7, 9, 11]])
+        self.assertAllEqual(output, [[5, 10, 6, 8], [5, 7, 9, 11]])
 
     def test_detokenize(self):
-        input_data = [[2, 10, 6, 8]]
+        input_data = [[5, 10, 6, 8]]
         output = self.tokenizer.detokenize(input_data)
         self.assertEqual(output, ["the quick brown fox"])
 
     def test_vocabulary_size(self):
-        tokenizer = FNetTokenizer(proto=self.proto)
+        tokenizer = AlbertTokenizer(proto=self.proto)
         self.assertEqual(tokenizer.vocabulary_size(), 12)
 
     def test_errors_missing_special_tokens(self):
         bytes_io = io.BytesIO()
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=iter(["abc"]),
             model_writer=bytes_io,
             vocab_size=5,
             pad_id=-1,
             eos_id=-1,
             bos_id=-1,
         )
         with self.assertRaises(ValueError):
-            FNetTokenizer(proto=bytes_io.getvalue())
+            AlbertTokenizer(proto=bytes_io.getvalue())
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.tokenizer)
         new_tokenizer = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_tokenizer.get_config(),
             self.tokenizer.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/generative_task.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/generative_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -180,20 +180,27 @@
         This function converts all output to numpy (for integer output), or
         python strings (for string output). If a batch dimension was added to
         the input, it is removed from the output (so generate can be string in,
         string out).
         """
 
         def normalize(x):
-            x = tf.concat(x, axis=0)
-            x = tf.squeeze(x, 0) if input_is_scalar else x
-            is_string = x.dtype == tf.string
-            # Convert outputs to a friendly pythonic type. For numerical outputs
-            # that is numpy, for string outputs that is `list` and `str`.
-            return tensor_to_list(x) if is_string else x.numpy()
+            if isinstance(x[0], list):
+                outputs = []
+                for batch in x:
+                    for e in batch:
+                        outputs.append(e)
+                return outputs[0] if input_is_scalar else outputs
+            if isinstance(x[0], tf.Tensor) and x[0].dtype == tf.string:
+                outputs = tf.concat(x, axis=0)
+                outputs = tf.squeeze(outputs, 0) if input_is_scalar else outputs
+                return tensor_to_list(outputs)
+            outputs = ops.concatenate(x, axis=0)
+            outputs = ops.squeeze(outputs, 0) if input_is_scalar else outputs
+            return ops.convert_to_numpy(outputs)
 
         if isinstance(outputs[0], dict):
             normalized = {}
             for key in outputs[0]:
                 normalized[key] = normalize([x[key] for x in outputs])
             return normalized
         return normalize([x for x in outputs])
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_backbone_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Test for GPT-2 backbone models."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
 from keras_nlp.src.models.gpt2.gpt2_backbone import GPT2Backbone
 from keras_nlp.src.tests.test_case import TestCase
 
 
 class GPT2Test(TestCase):
     def setUp(self):
         self.backbone = GPT2Backbone(
@@ -31,17 +31,17 @@
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
         )
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "segment_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "segment_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_call(self):
         self.backbone(self.input_batch)
@@ -53,16 +53,16 @@
     def test_name(self):
         # Check default name passed through
         self.assertRegexpMatches(self.backbone.name, "gpt2_backbone")
 
     def test_variable_sequence_length(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "padding_mask": ops.ones((2, seq_length), dtype="int32"),
+                "token_ids": np.ones((2, seq_length), dtype="int32"),
+                "padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
             self.backbone(input_data)
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
@@ -114,16 +114,16 @@
                 num_layers=2,
                 num_heads=2,
                 hidden_dim=2,
                 intermediate_dim=4,
                 max_sequence_length=5,
             )
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.model.compile()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,15 +325,18 @@
             hidden_states=hidden_states,
         )
 
         # Compute an output padding mask with the token ids we updated.
         if end_token_id is not None:
             # Build a mask of `end_token_id` locations not in the original
             # prompt (not in locations where `padding_mask` is True).
-            end_locations = (token_ids == end_token_id) & (~padding_mask)
+            end_locations = ops.logical_and(
+                ops.equal(token_ids, end_token_id),
+                ops.logical_not(padding_mask),
+            )
             end_locations = ops.cast(end_locations, "int32")
             # Use cumsum to get ones in all locations after end_locations.
             cumsum = ops.cast(ops.cumsum(end_locations, axis=-1), "int32")
             overflow = cumsum - end_locations
             # Our padding mask is the inverse of these overflow locations.
             padding_mask = ops.logical_not(ops.cast(overflow, "bool"))
         else:
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,141 +8,123 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for GPT2 causal LM preprocessor layer."""
-import os
+"""Tests for OPT causal LM preprocessor layer."""
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.gpt2.gpt2_causal_lm_preprocessor import (
-    GPT2CausalLMPreprocessor,
+from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import (
+    OPTCausalLMPreprocessor,
 )
-from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class GPT2CausalLMPreprocessorTest(TestCase):
+class OPTCausalLMPreprocessorTest(TestCase):
     def setUp(self):
         self.vocab = {
-            "!": 0,
-            "air": 1,
-            "Ġair": 2,
-            "plane": 3,
-            "Ġat": 4,
-            "port": 5,
-            "<|endoftext|>": 6,
+            "<pad>": 0,
+            "</s>": 1,
+            "air": 2,
+            "Ġair": 3,
+            "plane": 4,
+            "Ġat": 5,
+            "port": 6,
         }
 
-        self.merges = ["Ġ a", "Ġ t", "Ġ i", "Ġ b", "a i", "p l", "n e"]
-        self.merges += ["Ġa t", "p o", "r t", "Ġt h", "ai r", "pl a", "po rt"]
-        self.merges += ["Ġai r", "Ġa i", "pla ne"]
+        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
+        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
+        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
+        merges += ["pla ne"]
+        self.merges = merges
 
-        self.preprocessor = GPT2CausalLMPreprocessor(
-            tokenizer=GPT2Tokenizer(
+        self.preprocessor = OPTCausalLMPreprocessor(
+            tokenizer=OPTTokenizer(
                 vocabulary=self.vocab,
                 merges=self.merges,
             ),
             sequence_length=8,
         )
 
     def test_strings(self):
-        input_data = "airplane at airport"
+        input_data = " airplane at airport"
 
         x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 6, 0])
+        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 1, 0])
         self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
-        self.assertAllEqual(y, [1, 3, 4, 2, 5, 6, 0, 0])
+        self.assertAllEqual(y, [3, 4, 5, 3, 6, 1, 0, 0])
         self.assertAllEqual(sw, [1, 1, 1, 1, 1, 1, 0, 0])
 
     def test_list_of_strings(self):
-        input_data = ["airplane at airport"] * 4
+        input_data = [" airplane at airport"] * 4
 
         x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
+        self.assertAllEqual(y, [[3, 4, 5, 3, 6, 1, 0, 0]] * 4)
         self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
 
     def test_no_start_end_token(self):
-        input_data = ["airplane at airport"] * 4
+        input_data = [" airplane at airport"] * 4
 
-        preprocessor = GPT2CausalLMPreprocessor(
-            tokenizer=GPT2Tokenizer(
+        preprocessor = OPTCausalLMPreprocessor(
+            tokenizer=OPTTokenizer(
                 vocabulary=self.vocab,
                 merges=self.merges,
             ),
             sequence_length=8,
             add_start_token=False,
             add_end_token=False,
         )
         x, y, sw = preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 2, 5, 0, 0, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[3, 4, 5, 3, 6, 0, 0, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
-        self.assertAllEqual(y, [[3, 4, 2, 5, 0, 0, 0, 0]] * 4)
+        self.assertAllEqual(y, [[4, 5, 3, 6, 0, 0, 0, 0]] * 4)
         self.assertAllEqual(sw, [[1, 1, 1, 1, 0, 0, 0, 0]] * 4)
 
     def test_labeled_batch(self):
-        x = tf.constant(["airplane at airport"] * 4)
+        x = tf.constant([" airplane at airport"] * 4)
         y = tf.constant([1] * 4)  # Ignored.
         sw = tf.constant([1.0] * 4)  # Ignored.
         x, y, sw = self.preprocessor(x, y, sw)
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
+        self.assertAllEqual(y, [[3, 4, 5, 3, 6, 1, 0, 0]] * 4)
         self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
 
     def test_dataset(self):
-        x = tf.constant(["airplane at airport"] * 4)
+        x = tf.constant([" airplane at airport"] * 4)
         ds = tf.data.Dataset.from_tensor_slices(x)
         ds = ds.map(self.preprocessor)
         x, y, sw = ds.batch(4).take(1).get_single_element()
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
+        self.assertAllEqual(y, [[3, 4, 5, 3, 6, 1, 0, 0]] * 4)
         self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
 
     def test_generate_preprocess(self):
-        input_data = "airplane at airport"
+        input_data = " airplane at airport"
         x = self.preprocessor.generate_preprocess(input_data)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 0, 0])
+        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 0, 0])
         self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0])
 
     def test_generate_postprocess(self):
         input_data = {
-            "token_ids": tf.constant([6, 1, 3, 4, 2, 5, 0, 0]),
+            "token_ids": tf.constant([1, 3, 4, 5, 3, 6, 0, 0]),
             "padding_mask": tf.cast([1, 1, 1, 1, 1, 1, 0, 0], dtype="bool"),
         }
         x = self.preprocessor.generate_postprocess(input_data)
-        self.assertAllEqual(x, "airplane at airport")
+        self.assertAllEqual(x, " airplane at airport")
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs, y, sw = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,123 +7,104 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Tests for DistilBERT preprocessor layer."""
 
-"""Tests for GPT2 preprocessor layer."""
-import os
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
-from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
+    DistilBertPreprocessor,
+)
+from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
+    DistilBertTokenizer,
+)
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class GPT2PreprocessorTest(TestCase):
+class DistilBertPreprocessorTest(TestCase):
     def setUp(self):
-        self.vocab = {
-            "!": 0,
-            "air": 1,
-            "Ġair": 2,
-            "plane": 3,
-            "Ġat": 4,
-            "port": 5,
-            "<|endoftext|>": 6,
-        }
-
-        self.merges = ["Ġ a", "Ġ t", "Ġ i", "Ġ b", "a i", "p l", "n e"]
-        self.merges += ["Ġa t", "p o", "r t", "Ġt h", "ai r", "pl a", "po rt"]
-        self.merges += ["Ġai r", "Ġa i", "pla ne"]
-
-        self.preprocessor = GPT2Preprocessor(
-            tokenizer=GPT2Tokenizer(
-                vocabulary=self.vocab,
-                merges=self.merges,
-            ),
+        self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
+        self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
+        self.vocab += ["the", "quick", "brown", "fox"]
+        self.preprocessor = DistilBertPreprocessor(
+            DistilBertTokenizer(vocabulary=self.vocab),
             sequence_length=8,
         )
 
     def test_tokenize_strings(self):
-        input_data = "airplane at airport"
-
-        x = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 6, 0])
-        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
+        input_data = "THE QUICK BROWN FOX."
+        output = self.preprocessor(input_data)
+        self.assertAllEqual(output["token_ids"], [2, 5, 6, 7, 8, 1, 3, 0])
+        self.assertAllEqual(output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
 
     def test_tokenize_list_of_strings(self):
-        input_data = ["airplane at airport"] * 4
-
-        x = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-
-    def test_no_start_end_token(self):
-        input_data = ["airplane at airport"] * 4
-
-        preprocessor = GPT2Preprocessor(
-            tokenizer=GPT2Tokenizer(
-                vocabulary=self.vocab,
-                merges=self.merges,
-            ),
-            sequence_length=8,
-            add_start_token=False,
-            add_end_token=False,
+        # We should handle a list of strings as as batch.
+        input_data = ["THE QUICK BROWN FOX."] * 4
+        output = self.preprocessor(input_data)
+        self.assertAllEqual(output["token_ids"], [[2, 5, 6, 7, 8, 1, 3, 0]] * 4)
+        self.assertAllEqual(
+            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4
         )
-        x = preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 2, 5, 0, 0, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
 
     def test_tokenize_labeled_batch(self):
-        x = tf.constant(["airplane at airport"] * 4)
-        y_in = tf.constant([1] * 4)
-        sw_in = tf.constant([1.0] * 4)
-        x, y, sw = self.preprocessor(x, y_in, sw_in)
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, y_in)
-        self.assertAllEqual(sw, sw_in)
+        x = tf.constant(["THE QUICK BROWN FOX."] * 4)
+        y = tf.constant([1] * 4)
+        sw = tf.constant([1.0] * 4)
+        x_out, y_out, sw_out = self.preprocessor(x, y, sw)
+        self.assertAllEqual(x_out["token_ids"], [[2, 5, 6, 7, 8, 1, 3, 0]] * 4)
+        self.assertAllEqual(
+            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4
+        )
+        self.assertAllEqual(y_out, y)
+        self.assertAllEqual(sw_out, sw)
 
     def test_tokenize_labeled_dataset(self):
-        x = tf.constant(["airplane at airport"] * 4)
-        ds = tf.data.Dataset.from_tensor_slices(x)
+        x = tf.constant(["THE QUICK BROWN FOX."] * 4)
+        y = tf.constant([1] * 4)
+        sw = tf.constant([1.0] * 4)
+        ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
         ds = ds.map(self.preprocessor)
-        x = ds.batch(4).take(1).get_single_element()
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-
-    def test_sequence_length_override(self):
-        input_data = "airplane at airport"
-        x = self.preprocessor(input_data, sequence_length=4)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 6])
+        x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(x_out["token_ids"], [[2, 5, 6, 7, 8, 1, 3, 0]] * 4)
+        self.assertAllEqual(
+            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4
+        )
+        self.assertAllEqual(y_out, y)
+        self.assertAllEqual(sw_out, sw)
+
+    def test_tokenize_multiple_sentences(self):
+        sentence_one = tf.constant("THE QUICK")
+        sentence_two = tf.constant("BROWN FOX.")
+        output = self.preprocessor((sentence_one, sentence_two))
+        self.assertAllEqual(output["token_ids"], [2, 5, 6, 3, 7, 8, 1, 3])
+        self.assertAllEqual(output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1])
+
+    def test_tokenize_multiple_batched_sentences(self):
+        sentence_one = tf.constant(["THE QUICK"] * 4)
+        sentence_two = tf.constant(["BROWN FOX."] * 4)
+        # The first tuple or list is always interpreted as an enumeration of
+        # separate sequences to concatenate.
+        output = self.preprocessor((sentence_one, sentence_two))
+        self.assertAllEqual(output["token_ids"], [[2, 5, 6, 3, 7, 8, 1, 3]] * 4)
+        self.assertAllEqual(
+            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1]] * 4
+        )
+
+    def test_errors_for_2d_list_input(self):
+        ambiguous_input = [["one", "two"], ["three", "four"]]
+        with self.assertRaises(ValueError):
+            self.preprocessor(ambiguous_input)
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,111 +8,105 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for GPT-2 preprocessing layers."""
-import os
+"""Tests for GPTNeoX preprocessor layer."""
+
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_preprocessor import (
+    GPTNeoXPreprocessor,
+)
+from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_tokenizer import GPTNeoXTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class GPT2TokenizerTest(TestCase):
+class GPTNeoXPreprocessorTest(TestCase):
     def setUp(self):
         self.vocab = {
-            "<|endoftext|>": 0,
-            "Ġair": 1,
-            "plane": 2,
-            "Ġat": 3,
-            "port": 4,
-            "Ġkoh": 5,
-            "li": 6,
-            "Ġis": 7,
-            "Ġthe": 8,
-            "Ġbest": 9,
+            "!": 0,
+            "air": 1,
+            "Ġair": 2,
+            "plane": 3,
+            "Ġat": 4,
+            "port": 5,
+            "<|endoftext|>": 6,
         }
-        self.merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
-        self.merges += [
-            "Ġa t",
-            "p o",
-            "r t",
-            "o h",
-            "l i",
-            "Ġi s",
-            "Ġb e",
-            "s t",
-        ]
-        self.merges += [
-            "Ġt h",
-            "Ġai r",
-            "pl a",
-            "Ġk oh",
-            "Ġth e",
-            "Ġbe st",
-            "po rt",
-        ]
-        self.merges += ["pla ne"]
 
-        self.tokenizer = GPT2Tokenizer(
-            vocabulary=self.vocab, merges=self.merges
+        self.merges = ["Ġ a", "Ġ t", "Ġ i", "Ġ b", "a i", "p l", "n e"]
+        self.merges += ["Ġa t", "p o", "r t", "Ġt h", "ai r", "pl a", "po rt"]
+        self.merges += ["Ġai r", "Ġa i", "pla ne"]
+
+        self.preprocessor = GPTNeoXPreprocessor(
+            tokenizer=GPTNeoXTokenizer(
+                vocabulary=self.vocab,
+                merges=self.merges,
+            ),
+            sequence_length=8,
         )
 
-    def test_tokenize(self):
-        input_data = " airplane at airport"
-        output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [1, 2, 3, 1, 4])
-
-    def test_tokenize_end_token(self):
-        input_data = " airplane at airport<|endoftext|>"
-        output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [1, 2, 3, 1, 4, 0])
-
-    def test_tokenize_batch(self):
-        input_data = [" airplane at airport", " kohli is the best"]
-        output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [[1, 2, 3, 1, 4], [5, 6, 7, 8, 9]])
-
-    def test_detokenize(self):
-        input_tokens = [1, 2, 3, 1, 4]
-        output = self.tokenizer.detokenize(input_tokens)
-        self.assertEqual(output, " airplane at airport")
-
-    def test_vocabulary_size(self):
-        self.assertEqual(self.tokenizer.vocabulary_size(), 10)
-
-    def test_errors_missing_special_tokens(self):
-        with self.assertRaises(ValueError):
-            GPT2Tokenizer(vocabulary=["a", "b", "c"], merges=[])
+    def test_tokenize_strings(self):
+        input_data = "airplane at airport"
 
-    def test_serialization(self):
-        config = keras.saving.serialize_keras_object(self.tokenizer)
-        new_tokenizer = keras.saving.deserialize_keras_object(config)
-        self.assertEqual(
-            new_tokenizer.get_config(),
-            self.tokenizer.get_config(),
+        x = self.preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 6, 0])
+        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
+
+    def test_tokenize_list_of_strings(self):
+        input_data = ["airplane at airport"] * 4
+
+        x = self.preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+
+    def test_no_start_end_token(self):
+        input_data = ["airplane at airport"] * 4
+
+        preprocessor = GPTNeoXPreprocessor(
+            tokenizer=GPTNeoXTokenizer(
+                vocabulary=self.vocab,
+                merges=self.merges,
+            ),
+            sequence_length=8,
+            add_start_token=False,
+            add_end_token=False,
         )
+        x = preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 2, 5, 0, 0, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
+
+    def test_tokenize_labeled_batch(self):
+        x = tf.constant(["airplane at airport"] * 4)
+        y_in = tf.constant([1] * 4)
+        sw_in = tf.constant([1.0] * 4)
+        x, y, sw = self.preprocessor(x, y_in, sw_in)
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(y, y_in)
+        self.assertAllEqual(sw, sw_in)
+
+    def test_tokenize_labeled_dataset(self):
+        x = tf.constant(["airplane at airport"] * 4)
+        ds = tf.data.Dataset.from_tensor_slices(x)
+        ds = ds.map(self.preprocessor)
+        x = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+
+    def test_sequence_length_override(self):
+        input_data = "airplane at airport"
+        x = self.preprocessor(input_data, sequence_length=4)
+        self.assertAllEqual(x["token_ids"], [6, 1, 3, 6])
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant([" airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
+    def test_serialization(self):
+        config = keras.saving.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.saving.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
         )
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_attention.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_attention.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import tensorflow as tf
 
 from keras_nlp.src.backend import keras
+from keras_nlp.src.backend import ops
 from keras_nlp.src.models.gpt_neo_x.rotary_embedding import RotaryEmbedding
 from keras_nlp.src.utils.keras_utils import clone_initializer
 
 
 class GPTNeoXAttention(keras.layers.Layer):
     """GPTNeoXAttention layer.
 
@@ -64,21 +64,23 @@
         self.rotary_max_wavelength = rotary_max_wavelength
         self.rotary_dim = int(self.attn_head_size * rotary_percentage)
         self.rotary_embedding = RotaryEmbedding(rotary_max_wavelength)
         self.kernel_initializer = keras.initializers.get(kernel_initializer)
         self.bias_initializer = keras.initializers.get(bias_initializer)
         self.max_sequence_length = max_sequence_length
 
+    def build(self, input_shape):
         self._qkv_dense = keras.layers.EinsumDense(
             equation="abc,cde->abde",
             output_shape=(None, self.num_heads, 3 * self.attn_head_size),
             bias_axes="de",
             **self._get_common_kwargs_for_sublayer(use_bias=True),
-            name="query",
+            name="query_key_value",
         )
+        self._qkv_dense.build(input_shape)
 
         self._attn_dropout_layer = keras.layers.Dropout(
             self.dropout, name="attention_dropout"
         )
 
         self._softmax = keras.layers.Softmax(axis=-1, name="attention_softmax")
 
@@ -87,14 +89,17 @@
             equation="abc,cd->abd",
             output_shape=(None, self.hidden_dim),
             bias_axes="d",
             **self._get_common_kwargs_for_sublayer(use_bias=True),
             name="attention_output",
         )
 
+        self._output_dense.build(input_shape)
+        self.built = True
+
     def _get_common_kwargs_for_sublayer(self, use_bias=True):
         common_kwargs = {}
 
         kernel_initializer = clone_initializer(self.kernel_initializer)
         bias_initializer = clone_initializer(self.bias_initializer)
 
         common_kwargs["kernel_initializer"] = kernel_initializer
@@ -103,89 +108,119 @@
 
         return common_kwargs
 
     def _masked_softmax(self, attention_scores, attention_mask=None):
         if attention_mask is not None:
             mask_expansion_axis = -3
             for _ in range(
-                attention_scores.shape.rank - attention_mask.shape.rank
+                len(attention_scores.shape) - len(attention_mask.shape)
             ):
-                attention_mask = tf.expand_dims(
+                attention_mask = ops.expand_dims(
                     attention_mask, axis=mask_expansion_axis
                 )
         return self._softmax(attention_scores, attention_mask)
 
     def _compute_attention(
         self, query, key, value, attention_mask=None, training=None
     ):
-        attention_scores = tf.einsum("aecd,abcd->acbe", key, query)
-        norm_factor = tf.sqrt(
-            tf.constant(self.attn_head_size, dtype=tf.float32)
+        attention_scores = ops.einsum("aecd,abcd->acbe", key, query)
+
+        norm_factor = ops.sqrt(
+            ops.convert_to_tensor(self.attn_head_size, self.compute_dtype)
         )
+
         attention_scores /= norm_factor
 
         attention_scores = self._masked_softmax(
             attention_scores, attention_mask
         )
         attention_scores = self._attn_dropout_layer(
             attention_scores, training=training
         )
-        attention_output = tf.einsum("acbe,aecd->abcd", attention_scores, value)
+        attention_output = ops.einsum(
+            "acbe,aecd->abcd", attention_scores, value
+        )
 
         return attention_output
 
     def call(
         self,
         hidden_states,
-        attention_mask,
+        attention_mask=None,
+        cache=None,
+        cache_update_index=None,
         training=None,
     ):
         query_key_value = self._qkv_dense(hidden_states)
 
         query = query_key_value[..., : self.attn_head_size]
-        key = query_key_value[
-            ..., self.attn_head_size : 2 * self.attn_head_size
-        ]
-        value = query_key_value[..., 2 * self.attn_head_size :]
+
+        if cache is not None:
+            key_cache = cache[:, 0, ...]
+            value_cache = cache[:, 1, ...]
+            if cache_update_index is None:
+                key = key_cache
+                value = value_cache
+            else:
+                key_update = query_key_value[
+                    ..., self.attn_head_size : 2 * self.attn_head_size
+                ]
+                value_update = query_key_value[..., 2 * self.attn_head_size :]
+                start = [0, cache_update_index, 0, 0]
+                key = ops.slice_update(key_cache, start, key_update)
+                value = ops.slice_update(value_cache, start, value_update)
+                cache = ops.stack((key, value), axis=1)
+        else:
+            if cache_update_index is not None:
+                raise ValueError(
+                    "`cache_update_index` should not be set if `cache` is "
+                    f"`None`. Received: cache={cache}, "
+                    f"cache_update_index={cache_update_index}"
+                )
+            key = query_key_value[
+                ..., self.attn_head_size : 2 * self.attn_head_size
+            ]
+            value = query_key_value[..., 2 * self.attn_head_size :]
 
         query_rot, query_pass = (
             query[..., : self.rotary_dim],
             query[..., self.rotary_dim :],
         )
         key_rot, key_pass = (
             key[..., : self.rotary_dim],
             key[..., self.rotary_dim :],
         )
 
-        query_rot, key_rot = self.rotary_embedding(query_rot, key_rot)
+        query_rot = self.rotary_embedding(query_rot)
+        key_rot = self.rotary_embedding(key_rot)
 
-        query = tf.concat((query_rot, query_pass), axis=-1)
-        key = tf.concat((key_rot, key_pass), axis=-1)
+        query = ops.concatenate((query_rot, query_pass), axis=-1)
+        key = ops.concatenate((key_rot, key_pass), axis=-1)
 
         attention_output = self._compute_attention(
             query=query,
             key=key,
             value=value,
             attention_mask=attention_mask,
             training=training,
         )
 
         # Reshape `attention_output` to `(batch_size, sequence_length, hidden_dim)`.
-        attention_output = tf.reshape(
+        attention_output = ops.reshape(
             attention_output,
             [
-                tf.shape(attention_output)[0],
-                tf.shape(attention_output)[1],
+                ops.shape(attention_output)[0],
+                ops.shape(attention_output)[1],
                 self.hidden_dim,
             ],
         )
 
         attention_output = self._output_dense(attention_output)
 
-        return attention_output
+        return attention_output, cache
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_heads": self.num_heads,
                 "hidden_dim": self.hidden_dim,
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+"""GPT-NeoX backbone model."""
+
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_decoder import GPTNeoXDecoder
-from keras_nlp.src.utils.tensor_utils import assert_tf_backend
 
 
 def _gpt_neo_x_kernel_initializer(stddev=0.02):
     return keras.initializers.RandomNormal(stddev=stddev)
 
 
 @keras.saving.register_keras_serializable(package="keras_nlp")
@@ -70,16 +72,14 @@
         dropout=0.0,
         rotary_percentage=0.25,
         rotary_max_wavelength=10000,
         layer_norm_epsilon=1e-5,
         max_sequence_length=512,
         **kwargs,
     ):
-        assert_tf_backend(self.__class__.__name__)
-
         # Inputs
         token_ids = keras.Input(shape=(None,), dtype="int32", name="token_ids")
         padding_mask = keras.Input(
             shape=(None,), dtype="int32", name="padding_mask"
         )
 
         # Embed tokens
@@ -131,27 +131,31 @@
         # All references to `self` below this line
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.hidden_dim = hidden_dim
         self.intermediate_dim = intermediate_dim
         self.dropout = dropout
+        self.rotary_percentage = rotary_percentage
+        self.rotary_max_wavelength = rotary_max_wavelength
         self.max_sequence_length = max_sequence_length
         self.layer_norm_epsilon = layer_norm_epsilon
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "vocabulary_size": self.vocabulary_size,
                 "num_layers": self.num_layers,
                 "num_heads": self.num_heads,
                 "hidden_dim": self.hidden_dim,
                 "intermediate_dim": self.intermediate_dim,
                 "dropout": self.dropout,
+                "rotary_percentage": self.rotary_percentage,
+                "rotary_max_wavelength": self.rotary_max_wavelength,
                 "max_sequence_length": self.max_sequence_length,
                 "layer_norm_epsilon": self.layer_norm_epsilon,
             }
         )
         return config
 
     @property
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,37 +11,36 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Test for GPTNeoX backbone models."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
 from keras_nlp.src.models import GPTNeoXBackbone
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
 class GPTNeoXTest(TestCase):
     def setUp(self):
         self.backbone = GPTNeoXBackbone(
             vocabulary_size=10,
             num_layers=4,
             num_heads=4,
             hidden_dim=64,
             intermediate_dim=64,
             max_sequence_length=10,
         )
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_call(self):
         self.backbone(self.input_batch)
@@ -53,16 +52,16 @@
     def test_name(self):
         # Check default name passed through
         self.assertRegexpMatches(self.backbone.name, "gpt_neo_x_backbone")
 
     def test_variable_sequence_length(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "padding_mask": ops.ones((2, seq_length), dtype="int32"),
+                "token_ids": np.ones((2, seq_length), dtype="int32"),
+                "padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
             self.backbone(input_data)
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
@@ -97,16 +96,16 @@
                 num_layers=4,
                 num_heads=4,
                 hidden_dim=64,
                 intermediate_dim=64,
                 max_sequence_length=10,
             )
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.model.compile()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
 @keras.saving.register_keras_serializable(package="keras_nlp")
 class GPTNeoXCausalLMPreprocessor(GPTNeoXPreprocessor):
-    """GPTNeoX Causal LM preprocessor.
+    """GPT-NeoX Causal LM preprocessor.
 
     This preprocessing layer is meant for use with
     `keras_nlp.models.GPTNeoXCausalLM`. By default, it will take in batches of
     strings, and return outputs in a `(x, y, sample_weight)` format, where the
     `y` label is the next token id in the `x` sequence.
 
     For use with generation, the layer also exposes two methods
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for GPTNeoX causal LM preprocessor layer."""
-import os
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_causal_lm_preprocessor import (
     GPTNeoXCausalLMPreprocessor,
 )
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_tokenizer import GPTNeoXTokenizer
@@ -124,25 +122,7 @@
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs, y, sw = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_decoder.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_decoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import tensorflow as tf
-
 from keras_nlp.src.backend import keras
+from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling.transformer_layer_utils import (
     compute_causal_mask,
 )
 from keras_nlp.src.layers.modeling.transformer_layer_utils import (
     merge_padding_and_attention_mask,
 )
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_attention import GPTNeoXAttention
@@ -65,111 +64,158 @@
         activation="relu",
         layer_norm_epsilon=1e-5,
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         rotary_percentage=0.25,
         rotary_max_wavelength=10000,
         max_sequence_length=512,
-        name=None,
         **kwargs,
     ):
-        super().__init__(name=name, **kwargs)
+        super().__init__(**kwargs)
         self.intermediate_dim = intermediate_dim
         self.num_heads = num_heads
         self.dropout = dropout
         self.rotary_percentage = rotary_percentage
         self.rotary_max_wavelength = rotary_max_wavelength
         self.max_sequence_length = max_sequence_length
         self.activation = keras.activations.get(activation)
         self.layer_norm_epsilon = layer_norm_epsilon
         self.kernel_initializer = keras.initializers.get(kernel_initializer)
         self.bias_initializer = keras.initializers.get(bias_initializer)
         self.supports_masking = True
         self.rotary_percentage = rotary_percentage
+        self._decoder_sequence_shape = None
 
-    def build(self, input_shape):
-        hidden_dim = input_shape[-1]
+    def build(self, decoder_sequence_shape):
+        self._decoder_sequence_shape = decoder_sequence_shape
+        hidden_dim = decoder_sequence_shape[-1]
         # Self attention layers.
         self._self_attention_layer = GPTNeoXAttention(
             num_heads=self.num_heads,
             hidden_dim=hidden_dim,
             dropout=self.dropout,
             rotary_percentage=self.rotary_percentage,
             rotary_max_wavelength=self.rotary_max_wavelength,
             max_sequence_length=self.max_sequence_length,
             kernel_initializer=clone_initializer(self.kernel_initializer),
             bias_initializer=clone_initializer(self.bias_initializer),
         )
+        self._self_attention_layer.build(decoder_sequence_shape)
 
         self._self_attention_layernorm = keras.layers.LayerNormalization(
             epsilon=self.layer_norm_epsilon,
         )
+        self._self_attention_layernorm.build(decoder_sequence_shape)
 
         self._self_attention_dropout = keras.layers.Dropout(
             rate=self.dropout,
         )
 
         # Feedforward layers.
         self._feedforward_intermediate_dense = keras.layers.Dense(
             self.intermediate_dim,
             activation=self.activation,
             kernel_initializer=clone_initializer(self.kernel_initializer),
             bias_initializer=clone_initializer(self.bias_initializer),
         )
+        self._feedforward_intermediate_dense.build(decoder_sequence_shape)
+
         self._feedforward_output_dense = keras.layers.Dense(
             hidden_dim,
             kernel_initializer=clone_initializer(self.kernel_initializer),
             bias_initializer=clone_initializer(self.bias_initializer),
         )
 
+        intermediate_shape = list(decoder_sequence_shape)
+        intermediate_shape[-1] = self.intermediate_dim
+        self._feedforward_output_dense.build(tuple(intermediate_shape))
+
         self._feedforward_layernorm = keras.layers.LayerNormalization(
             epsilon=self.layer_norm_epsilon,
         )
+        self._feedforward_layernorm.build(decoder_sequence_shape)
 
         self._feedforward_dropout = keras.layers.Dropout(
             rate=self.dropout,
         )
+        self.built = True
 
     def call(
         self,
         decoder_sequence,
         decoder_padding_mask=None,
         decoder_attention_mask=None,
+        self_attention_cache=None,
+        self_attention_cache_update_index=None,
     ):
-        # Compute self attention mask.
-        batch_size = tf.shape(decoder_sequence)[0]
-        input_length = output_length = tf.shape(decoder_sequence)[1]
-
-        self_attention_mask = compute_causal_mask(
-            batch_size, input_length, output_length, 0
+        self_attention_mask = self._compute_self_attention_mask(
+            decoder_sequence=decoder_sequence,
+            decoder_padding_mask=decoder_padding_mask,
+            decoder_attention_mask=decoder_attention_mask,
+            self_attention_cache=self_attention_cache,
+            self_attention_cache_update_index=self_attention_cache_update_index,
         )
-        decoder_mask = merge_padding_and_attention_mask(
-            decoder_sequence, decoder_padding_mask, decoder_attention_mask
-        )
-        if decoder_mask is not None:
-            self_attention_mask = tf.minimum(decoder_mask, self_attention_mask)
 
         residual = decoder_sequence
 
         x = self._self_attention_layernorm(decoder_sequence)
 
         # Self attention block.
-        x = self._self_attention_layer(
+        x, self_attention_cache = self._self_attention_layer(
             hidden_states=x,
             attention_mask=self_attention_mask,
+            cache=self_attention_cache,
+            cache_update_index=self_attention_cache_update_index,
         )
         x = self._self_attention_dropout(x)
         attention_output = x
 
         x = self._feedforward_layernorm(decoder_sequence)
         x = self._feedforward_intermediate_dense(x)
         x = self._feedforward_output_dense(x)
         feedforward_output = x
+        x = feedforward_output + attention_output + residual
+
+        if self_attention_cache is not None:
+            return (x, self_attention_cache)
+        else:
+            return x
 
-        return feedforward_output + attention_output + residual
+    def _compute_self_attention_mask(
+        self,
+        decoder_sequence,
+        decoder_padding_mask,
+        decoder_attention_mask,
+        self_attention_cache=None,
+        self_attention_cache_update_index=None,
+    ):
+        decoder_mask = merge_padding_and_attention_mask(
+            decoder_sequence, decoder_padding_mask, decoder_attention_mask
+        )
+        batch_size = ops.shape(decoder_sequence)[0]
+        input_length = output_length = ops.shape(decoder_sequence)[1]
+        # We need to handle a rectangular causal mask when doing cached
+        # decoding. For generative inference, `decoder_sequence` will
+        # generally be length 1, and `cache` will be the full generation length.
+        if self_attention_cache is not None:
+            input_length = ops.shape(self_attention_cache)[2]
+
+        causal_mask = compute_causal_mask(
+            batch_size,
+            input_length,
+            output_length,
+            0
+            if self_attention_cache_update_index is None
+            else self_attention_cache_update_index,
+        )
+        return (
+            ops.minimum(decoder_mask, causal_mask)
+            if decoder_mask is not None
+            else causal_mask
+        )
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "intermediate_dim": self.intermediate_dim,
                 "num_heads": self.num_heads,
@@ -181,11 +227,15 @@
                 "layer_norm_epsilon": self.layer_norm_epsilon,
                 "kernel_initializer": keras.initializers.serialize(
                     self.kernel_initializer
                 ),
                 "bias_initializer": keras.initializers.serialize(
                     self.bias_initializer
                 ),
+                "decoder_sequence_shape": self._decoder_sequence_shape,
             }
         )
         return config
 
+    def compute_output_shape(self, decoder_sequence_shape):
+        return decoder_sequence_shape
+
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_preprocessor_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,125 +8,104 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for GPTNeoX preprocessor layer."""
+"""Tests for OPT preprocessor layer."""
 
-import os
-
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_preprocessor import (
-    GPTNeoXPreprocessor,
-)
-from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_tokenizer import GPTNeoXTokenizer
+from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
+from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class GPTNeoXPreprocessorTest(TestCase):
+class OPTPreprocessorTest(TestCase):
     def setUp(self):
         self.vocab = {
-            "!": 0,
-            "air": 1,
-            "Ġair": 2,
-            "plane": 3,
-            "Ġat": 4,
-            "port": 5,
-            "<|endoftext|>": 6,
+            "<pad>": 0,
+            "</s>": 1,
+            "air": 2,
+            "Ġair": 3,
+            "plane": 4,
+            "Ġat": 5,
+            "port": 6,
         }
 
-        self.merges = ["Ġ a", "Ġ t", "Ġ i", "Ġ b", "a i", "p l", "n e"]
-        self.merges += ["Ġa t", "p o", "r t", "Ġt h", "ai r", "pl a", "po rt"]
-        self.merges += ["Ġai r", "Ġa i", "pla ne"]
+        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
+        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
+        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
+        merges += ["pla ne"]
+        self.merges = merges
 
-        self.preprocessor = GPTNeoXPreprocessor(
-            tokenizer=GPTNeoXTokenizer(
+        self.preprocessor = OPTPreprocessor(
+            tokenizer=OPTTokenizer(
                 vocabulary=self.vocab,
                 merges=self.merges,
             ),
             sequence_length=8,
         )
 
     def test_tokenize_strings(self):
-        input_data = "airplane at airport"
+        input_data = " airplane at airport"
 
         x = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 6, 0])
+        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 1, 0])
         self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
 
     def test_tokenize_list_of_strings(self):
-        input_data = ["airplane at airport"] * 4
+        input_data = [" airplane at airport"] * 4
 
         x = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
 
     def test_no_start_end_token(self):
-        input_data = ["airplane at airport"] * 4
+        input_data = [" airplane at airport"] * 4
 
-        preprocessor = GPTNeoXPreprocessor(
-            tokenizer=GPTNeoXTokenizer(
+        preprocessor = OPTPreprocessor(
+            tokenizer=OPTTokenizer(
                 vocabulary=self.vocab,
                 merges=self.merges,
             ),
             sequence_length=8,
             add_start_token=False,
             add_end_token=False,
         )
         x = preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 2, 5, 0, 0, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[3, 4, 5, 3, 6, 0, 0, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
 
     def test_tokenize_labeled_batch(self):
-        x = tf.constant(["airplane at airport"] * 4)
+        x = tf.constant([" airplane at airport"] * 4)
         y_in = tf.constant([1] * 4)
         sw_in = tf.constant([1.0] * 4)
         x, y, sw = self.preprocessor(x, y_in, sw_in)
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
         self.assertAllEqual(y, y_in)
         self.assertAllEqual(sw, sw_in)
 
     def test_tokenize_labeled_dataset(self):
-        x = tf.constant(["airplane at airport"] * 4)
+        x = tf.constant([" airplane at airport"] * 4)
         ds = tf.data.Dataset.from_tensor_slices(x)
         ds = ds.map(self.preprocessor)
         x = ds.batch(4).take(1).get_single_element()
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
 
     def test_sequence_length_override(self):
-        input_data = "airplane at airport"
+        input_data = " airplane at airport"
         x = self.preprocessor(input_data, sequence_length=4)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 6])
+        self.assertAllEqual(x["token_ids"], [1, 3, 4, 1])
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,111 +8,102 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for GPT-2 preprocessing layers."""
-import os
+"""Tests for GPT2 preprocessor layer."""
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_tokenizer import GPTNeoXTokenizer
+from keras_nlp.src.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
+from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class GPTNeoXTokenizerTest(TestCase):
+class GPT2PreprocessorTest(TestCase):
     def setUp(self):
         self.vocab = {
-            "<|endoftext|>": 0,
-            "Ġair": 1,
-            "plane": 2,
-            "Ġat": 3,
-            "port": 4,
-            "Ġkoh": 5,
-            "li": 6,
-            "Ġis": 7,
-            "Ġthe": 8,
-            "Ġbest": 9,
+            "!": 0,
+            "air": 1,
+            "Ġair": 2,
+            "plane": 3,
+            "Ġat": 4,
+            "port": 5,
+            "<|endoftext|>": 6,
         }
-        self.merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
-        self.merges += [
-            "Ġa t",
-            "p o",
-            "r t",
-            "o h",
-            "l i",
-            "Ġi s",
-            "Ġb e",
-            "s t",
-        ]
-        self.merges += [
-            "Ġt h",
-            "Ġai r",
-            "pl a",
-            "Ġk oh",
-            "Ġth e",
-            "Ġbe st",
-            "po rt",
-        ]
-        self.merges += ["pla ne"]
 
-        self.tokenizer = GPTNeoXTokenizer(
-            vocabulary=self.vocab, merges=self.merges
+        self.merges = ["Ġ a", "Ġ t", "Ġ i", "Ġ b", "a i", "p l", "n e"]
+        self.merges += ["Ġa t", "p o", "r t", "Ġt h", "ai r", "pl a", "po rt"]
+        self.merges += ["Ġai r", "Ġa i", "pla ne"]
+
+        self.preprocessor = GPT2Preprocessor(
+            tokenizer=GPT2Tokenizer(
+                vocabulary=self.vocab,
+                merges=self.merges,
+            ),
+            sequence_length=8,
         )
 
-    def test_tokenize(self):
-        input_data = " airplane at airport"
-        output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [1, 2, 3, 1, 4])
-
-    def test_tokenize_end_token(self):
-        input_data = " airplane at airport<|endoftext|>"
-        output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [1, 2, 3, 1, 4, 0])
-
-    def test_tokenize_batch(self):
-        input_data = [" airplane at airport", " kohli is the best"]
-        output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [[1, 2, 3, 1, 4], [5, 6, 7, 8, 9]])
-
-    def test_detokenize(self):
-        input_tokens = [1, 2, 3, 1, 4]
-        output = self.tokenizer.detokenize(input_tokens)
-        self.assertEqual(output, " airplane at airport")
-
-    def test_vocabulary_size(self):
-        self.assertEqual(self.tokenizer.vocabulary_size(), 10)
-
-    def test_errors_missing_special_tokens(self):
-        with self.assertRaises(ValueError):
-            GPTNeoXTokenizer(vocabulary=["a", "b", "c"], merges=[])
+    def test_tokenize_strings(self):
+        input_data = "airplane at airport"
 
-    def test_serialization(self):
-        config = keras.saving.serialize_keras_object(self.tokenizer)
-        new_tokenizer = keras.saving.deserialize_keras_object(config)
-        self.assertEqual(
-            new_tokenizer.get_config(),
-            self.tokenizer.get_config(),
+        x = self.preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 6, 0])
+        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
+
+    def test_tokenize_list_of_strings(self):
+        input_data = ["airplane at airport"] * 4
+
+        x = self.preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+
+    def test_no_start_end_token(self):
+        input_data = ["airplane at airport"] * 4
+
+        preprocessor = GPT2Preprocessor(
+            tokenizer=GPT2Tokenizer(
+                vocabulary=self.vocab,
+                merges=self.merges,
+            ),
+            sequence_length=8,
+            add_start_token=False,
+            add_end_token=False,
         )
+        x = preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 2, 5, 0, 0, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
+
+    def test_tokenize_labeled_batch(self):
+        x = tf.constant(["airplane at airport"] * 4)
+        y_in = tf.constant([1] * 4)
+        sw_in = tf.constant([1.0] * 4)
+        x, y, sw = self.preprocessor(x, y_in, sw_in)
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(y, y_in)
+        self.assertAllEqual(sw, sw_in)
+
+    def test_tokenize_labeled_dataset(self):
+        x = tf.constant(["airplane at airport"] * 4)
+        ds = tf.data.Dataset.from_tensor_slices(x)
+        ds = ds.map(self.preprocessor)
+        x = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+
+    def test_sequence_length_override(self):
+        input_data = "airplane at airport"
+        x = self.preprocessor(input_data, sequence_length=4)
+        self.assertAllEqual(x["token_ids"], [6, 1, 3, 6])
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant([" airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
+    def test_serialization(self):
+        config = keras.saving.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.saving.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
         )
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_backbone_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,125 +7,135 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for OPT backbone models."""
+"""Test for T5 backbone model."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
-from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
+from keras_nlp.src.models.t5.t5_backbone import T5Backbone
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class OPTBackboneTest(TestCase):
+@pytest.mark.tf_only
+class T5Test(TestCase):
     def setUp(self):
-        self.backbone = OPTBackbone(
-            vocabulary_size=10,
+        self.backbone = T5Backbone(
+            vocabulary_size=4,
             num_layers=2,
             num_heads=2,
-            hidden_dim=2,
+            hidden_dim=4,
             intermediate_dim=4,
-            max_sequence_length=5,
         )
+        self.batch_size = 2
+        seq_length = 3
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "encoder_token_ids": np.ones(
+                (self.batch_size, seq_length), dtype="int32"
+            ),
+            "encoder_padding_mask": np.ones(
+                (self.batch_size, seq_length), dtype="int32"
+            ),
+            "decoder_token_ids": np.ones(
+                (self.batch_size, seq_length), dtype="int32"
+            ),
+            "decoder_padding_mask": np.ones(
+                (self.batch_size, seq_length), dtype="int32"
+            ),
         }
-
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
-    def test_valid_call_opt(self):
+    def test_valid_call_t5(self):
         self.backbone(self.input_batch)
 
     def test_token_embedding(self):
-        output = self.backbone.token_embedding(self.input_batch["token_ids"])
-        self.assertEqual(output.shape, (2, 5, 2))
+        output = self.backbone.token_embedding(
+            self.input_batch["encoder_token_ids"]
+        )
+        self.assertEqual(output.shape, (2, 3, 4))
 
     def test_name(self):
         # Check default name passed through
-        self.assertRegexpMatches(self.backbone.name, "opt_backbone")
+        self.assertRegexpMatches(self.backbone.name, "t5_backbone")
 
-    def test_variable_sequence_length_call_opt(self):
+    def test_variable_sequence_length_call_t5(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "padding_mask": ops.ones((2, seq_length), dtype="int32"),
+                "encoder_token_ids": np.ones(
+                    (self.batch_size, seq_length), dtype="int32"
+                ),
+                "encoder_padding_mask": np.ones(
+                    (self.batch_size, seq_length), dtype="int32"
+                ),
+                "decoder_token_ids": np.ones(
+                    (self.batch_size, seq_length), dtype="int32"
+                ),
+                "decoder_padding_mask": np.ones(
+                    (self.batch_size, seq_length), dtype="int32"
+                ),
             }
-            self.backbone(input_data)
+            outputs = self.backbone(input_data)
+            self.assertIn("encoder_sequence_output", outputs)
+            self.assertIn("decoder_sequence_output", outputs)
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
     def test_serialization(self):
         new_backbone = keras.saving.deserialize_keras_object(
             keras.saving.serialize_keras_object(self.backbone)
         )
         self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
     @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self):
-        model_output = self.backbone(self.input_batch)
+        outputs = self.backbone(self.input_batch)
         path = os.path.join(self.get_temp_dir(), "model.keras")
         self.backbone.save(path, save_format="keras_v3")
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, OPTBackbone)
+        self.assertIsInstance(restored_model, T5Backbone)
 
         # Check that output matches.
-        restored_output = restored_model(self.input_batch)
-        self.assertAllClose(model_output, restored_output)
-
-    def test_create_layout_map(self):
-        mesh = tf.experimental.dtensor.create_mesh([("batch", 1), ("model", 1)])
-        with OPTBackbone.create_layout_map(mesh).scope():
-            OPTBackbone(
-                vocabulary_size=10,
-                num_layers=2,
-                num_heads=2,
-                hidden_dim=2,
-                intermediate_dim=4,
-                max_sequence_length=5,
-            )
-        # Using DTensor enables the mlir bridge as a side effect. Eventually
-        # this will be default, but for now we have compile errors with the
-        # bridge elsewhere and must disable. See
-        # https://github.com/keras-team/keras-nlp/issues/1001
-        tf.config.experimental.disable_mlir_bridge()
+        restored_outputs = restored_model(self.input_batch)
+        for key in ["encoder_sequence_output", "decoder_sequence_output"]:
+            self.assertAllClose(outputs[key], restored_outputs[key])
 
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
-class OPTBackboneTPUTest(TestCase):
+class T5BackboneTPUTest(TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
-            self.backbone = OPTBackbone(
-                vocabulary_size=1000,
+            self.backbone = T5Backbone(
+                vocabulary_size=4,
                 num_layers=2,
                 num_heads=2,
-                hidden_dim=32,
-                intermediate_dim=128,
-                max_sequence_length=128,
+                hidden_dim=4,
+                intermediate_dim=4,
             )
         self.input_batch = {
-            "token_ids": ops.ones((8, 128), dtype="int32"),
-            "padding_mask": ops.ones((8, 128), dtype="int32"),
+            "token_ids": np.ones((8, 4), dtype="int32"),
+            "padding_mask": np.ones((8, 4), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
-        self.backbone.predict(self.input_dataset)
+        outputs = self.backbone.predict(self.input_dataset)
+        self.assertIn("encoder_sequence_output", outputs)
+        self.assertIn("decoder_sequence_output", outputs)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_causal_lm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_causal_lm.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,18 @@
             hidden_states=hidden_states,
         )
 
         # Compute an output padding mask with the token ids we updated.
         if end_token_id is not None:
             # Build a mask of `end_token_id` locations not in the original
             # prompt (not in locations where `padding_mask` is True).
-            end_locations = (token_ids == end_token_id) & (~padding_mask)
+            end_locations = ops.logical_and(
+                ops.equal(token_ids, end_token_id),
+                ops.logical_not(padding_mask),
+            )
             end_locations = ops.cast(end_locations, "int32")
             # Use cumsum to get ones in all locations after end_locations.
             cumsum = ops.cast(ops.cumsum(end_locations, axis=-1), "int32")
             overflow = cumsum - end_locations
             # Our padding mask is the inverse of these overflow locations.
             padding_mask = ops.logical_not(ops.cast(overflow, "bool"))
         else:
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,143 +8,133 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for OPT causal LM preprocessor layer."""
-import os
+"""Tests for XLM-RoBERTa preprocessor layer."""
+import io
 
-import pytest
+import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import (
-    OPTCausalLMPreprocessor,
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import (
+    XLMRobertaPreprocessor,
+)
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
+    XLMRobertaTokenizer,
 )
-from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class OPTCausalLMPreprocessorTest(TestCase):
+class XLMRobertaPreprocessorTest(TestCase):
     def setUp(self):
-        self.vocab = {
-            "<pad>": 0,
-            "</s>": 1,
-            "air": 2,
-            "Ġair": 3,
-            "plane": 4,
-            "Ġat": 5,
-            "port": 6,
-        }
-
-        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
-        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
-        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
-        merges += ["pla ne"]
-        self.merges = merges
-
-        self.preprocessor = OPTCausalLMPreprocessor(
-            tokenizer=OPTTokenizer(
-                vocabulary=self.vocab,
-                merges=self.merges,
-            ),
-            sequence_length=8,
-        )
-
-    def test_strings(self):
-        input_data = " airplane at airport"
-
-        x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 1, 0])
-        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
-        self.assertAllEqual(y, [3, 4, 5, 3, 6, 1, 0, 0])
-        self.assertAllEqual(sw, [1, 1, 1, 1, 1, 1, 0, 0])
-
-    def test_list_of_strings(self):
-        input_data = [" airplane at airport"] * 4
-
-        x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, [[3, 4, 5, 3, 6, 1, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
-
-    def test_no_start_end_token(self):
-        input_data = [" airplane at airport"] * 4
-
-        preprocessor = OPTCausalLMPreprocessor(
-            tokenizer=OPTTokenizer(
-                vocabulary=self.vocab,
-                merges=self.merges,
-            ),
-            sequence_length=8,
-            add_start_token=False,
-            add_end_token=False,
-        )
-        x, y, sw = preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[3, 4, 5, 3, 6, 0, 0, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
-        self.assertAllEqual(y, [[4, 5, 3, 6, 0, 0, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 0, 0, 0, 0]] * 4)
-
-    def test_labeled_batch(self):
-        x = tf.constant([" airplane at airport"] * 4)
-        y = tf.constant([1] * 4)  # Ignored.
-        sw = tf.constant([1.0] * 4)  # Ignored.
-        x, y, sw = self.preprocessor(x, y, sw)
-        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, [[3, 4, 5, 3, 6, 1, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
-
-    def test_dataset(self):
-        x = tf.constant([" airplane at airport"] * 4)
-        ds = tf.data.Dataset.from_tensor_slices(x)
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the earth is round"]
+        )
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=10,
+            model_type="WORD",
+            unk_id=0,
+            bos_id=1,
+            eos_id=2,
+        )
+        self.proto = bytes_io.getvalue()
+
+        self.preprocessor = XLMRobertaPreprocessor(
+            tokenizer=XLMRobertaTokenizer(proto=self.proto),
+            sequence_length=12,
+        )
+
+    def test_tokenize_strings(self):
+        input_data = "the quick brown fox"
+        output = self.preprocessor(input_data)
+        self.assertAllEqual(
+            output["token_ids"], [0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]
+        )
+        self.assertAllEqual(
+            output["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
+        )
+
+    def test_tokenize_list_of_strings(self):
+        # We should handle a list of strings as as batch.
+        input_data = ["the quick brown fox"] * 4
+        output = self.preprocessor(input_data)
+        self.assertAllEqual(
+            output["token_ids"], [[0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]] * 4
+        )
+        self.assertAllEqual(
+            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
+        )
+
+    def test_tokenize_labeled_batch(self):
+        x = tf.constant(["the quick brown fox"] * 4)
+        y = tf.constant([1] * 4)
+        sw = tf.constant([1.0] * 4)
+        x_out, y_out, sw_out = self.preprocessor(x, y, sw)
+        self.assertAllEqual(
+            x_out["token_ids"], [[0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]] * 4
+        )
+        self.assertAllEqual(
+            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(y_out, y)
+        self.assertAllEqual(sw_out, sw)
+
+    def test_tokenize_labeled_dataset(self):
+        x = tf.constant(["the quick brown fox"] * 4)
+        y = tf.constant([1] * 4)
+        sw = tf.constant([1.0] * 4)
+        ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
         ds = ds.map(self.preprocessor)
-        x, y, sw = ds.batch(4).take(1).get_single_element()
-        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, [[3, 4, 5, 3, 6, 1, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
-
-    def test_generate_preprocess(self):
-        input_data = " airplane at airport"
-        x = self.preprocessor.generate_preprocess(input_data)
-        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 0, 0])
-        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0])
-
-    def test_generate_postprocess(self):
-        input_data = {
-            "token_ids": tf.constant([1, 3, 4, 5, 3, 6, 0, 0]),
-            "padding_mask": tf.cast([1, 1, 1, 1, 1, 1, 0, 0], dtype="bool"),
-        }
-        x = self.preprocessor.generate_postprocess(input_data)
-        self.assertAllEqual(x, " airplane at airport")
+        x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(
+            x_out["token_ids"], [[0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]] * 4
+        )
+        self.assertAllEqual(
+            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(y_out, y)
+        self.assertAllEqual(sw_out, sw)
+
+    def test_tokenize_multiple_sentences(self):
+        sentence_one = tf.constant("the quick brown fox")
+        sentence_two = tf.constant("the earth")
+        output = self.preprocessor((sentence_one, sentence_two))
+        self.assertAllEqual(
+            output["token_ids"], [0, 4, 9, 5, 7, 2, 2, 4, 6, 2, 1, 1]
+        )
+        self.assertAllEqual(
+            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]
+        )
+
+    def test_tokenize_multiple_batched_sentences(self):
+        sentence_one = tf.constant(["the quick brown fox"] * 4)
+        sentence_two = tf.constant(["the earth"] * 4)
+        # The first tuple or list is always interpreted as an enumeration of
+        # separate sequences to concatenate.
+        output = self.preprocessor((sentence_one, sentence_two))
+        self.assertAllEqual(
+            output["token_ids"], [[0, 4, 9, 5, 7, 2, 2, 4, 6, 2, 1, 1]] * 4
+        )
+        self.assertAllEqual(
+            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 4
+        )
+
+    def test_errors_for_2d_list_input(self):
+        ambiguous_input = [["one", "two"], ["three", "four"]]
+        with self.assertRaises(ValueError):
+            self.preprocessor(ambiguous_input)
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant([" airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs, y, sw = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_causal_lm_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_causal_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_preprocessor_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,124 +8,140 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for OPT preprocessor layer."""
-import os
+"""Tests for RoBERTa preprocessor layer."""
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
-from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
+from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
+from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class OPTPreprocessorTest(TestCase):
+class RobertaPreprocessorTest(TestCase):
     def setUp(self):
-        self.vocab = {
-            "<pad>": 0,
-            "</s>": 1,
-            "air": 2,
+        vocab = {
+            "<s>": 0,
+            "<pad>": 1,
+            "</s>": 2,
             "Ġair": 3,
             "plane": 4,
             "Ġat": 5,
             "port": 6,
+            "Ġkoh": 7,
+            "li": 8,
+            "Ġis": 9,
+            "Ġthe": 10,
+            "Ġbest": 11,
+            "<mask>": 12,
         }
 
         merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
         merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
         merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
         merges += ["pla ne"]
-        self.merges = merges
 
-        self.preprocessor = OPTPreprocessor(
-            tokenizer=OPTTokenizer(
-                vocabulary=self.vocab,
-                merges=self.merges,
+        self.preprocessor = RobertaPreprocessor(
+            tokenizer=RobertaTokenizer(
+                vocabulary=vocab,
+                merges=merges,
             ),
-            sequence_length=8,
+            sequence_length=12,
         )
 
     def test_tokenize_strings(self):
         input_data = " airplane at airport"
 
-        x = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 1, 0])
-        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
+        output = self.preprocessor(input_data)
+        self.assertAllEqual(
+            output["token_ids"], [0, 3, 4, 5, 3, 6, 2, 1, 1, 1, 1, 1]
+        )
+        self.assertAllEqual(
+            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]
+        )
 
     def test_tokenize_list_of_strings(self):
         input_data = [" airplane at airport"] * 4
 
-        x = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-
-    def test_no_start_end_token(self):
-        input_data = [" airplane at airport"] * 4
+        output = self.preprocessor(input_data)
+        self.assertAllEqual(
+            output["token_ids"],
+            [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1, 1, 1]] * 4,
+        )
 
-        preprocessor = OPTPreprocessor(
-            tokenizer=OPTTokenizer(
-                vocabulary=self.vocab,
-                merges=self.merges,
-            ),
-            sequence_length=8,
-            add_start_token=False,
-            add_end_token=False,
-        )
-        x = preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[3, 4, 5, 3, 6, 0, 0, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
+        self.assertAllEqual(
+            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]] * 4
+        )
 
     def test_tokenize_labeled_batch(self):
         x = tf.constant([" airplane at airport"] * 4)
-        y_in = tf.constant([1] * 4)
-        sw_in = tf.constant([1.0] * 4)
-        x, y, sw = self.preprocessor(x, y_in, sw_in)
-        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, y_in)
-        self.assertAllEqual(sw, sw_in)
+        y = tf.constant([1] * 4)
+        sw = tf.constant([1.0] * 4)
+        x_out, y_out, sw_out = self.preprocessor(x, y, sw)
+        self.assertAllEqual(
+            x_out["token_ids"], [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1, 1, 1]] * 4
+        )
+        self.assertAllEqual(
+            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(y_out, y)
+        self.assertAllEqual(sw_out, sw)
 
     def test_tokenize_labeled_dataset(self):
         x = tf.constant([" airplane at airport"] * 4)
-        ds = tf.data.Dataset.from_tensor_slices(x)
+        y = tf.constant([1] * 4)
+        sw = tf.constant([1.0] * 4)
+        ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
         ds = ds.map(self.preprocessor)
-        x = ds.batch(4).take(1).get_single_element()
-        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(
+            x_out["token_ids"], [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1, 1, 1]] * 4
+        )
+        self.assertAllEqual(
+            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(y_out, y)
+        self.assertAllEqual(sw_out, sw)
 
-    def test_sequence_length_override(self):
-        input_data = " airplane at airport"
-        x = self.preprocessor(input_data, sequence_length=4)
-        self.assertAllEqual(x["token_ids"], [1, 3, 4, 1])
+    def test_tokenize_multiple_sentences(self):
+        sentence_one = tf.constant(" airplane at airport")
+        sentence_two = tf.constant(" kohli is the best")
+
+        output = self.preprocessor((sentence_one, sentence_two))
+        self.assertAllEqual(
+            output["token_ids"], [0, 3, 4, 5, 3, 2, 2, 7, 8, 9, 10, 2]
+        )
+        self.assertAllEqual(
+            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
+        )
+
+    def test_tokenize_multiple_batched_sentences(self):
+        sentence_one = tf.constant([" airplane at airport"] * 4)
+        sentence_two = tf.constant([" kohli is the best"] * 4)
+
+        output = self.preprocessor((sentence_one, sentence_two))
+        self.assertAllEqual(
+            output["token_ids"],
+            [[0, 3, 4, 5, 3, 2, 2, 7, 8, 9, 10, 2]] * 4,
+        )
+        self.assertAllEqual(
+            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]] * 4
+        )
+
+    def test_errors_for_2d_list_input(self):
+        ambiguous_input = [["one", "two"], ["three", "four"]]
+        with self.assertRaises(ValueError):
+            self.preprocessor(ambiguous_input)
 
     def test_serialization(self):
         config = keras.saving.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant([" airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/opt/opt_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/opt/opt_tokenizer_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for OPT tokenizer layer."""
-import os
 
-import pytest
-import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
 class OPTTokenizerTest(TestCase):
@@ -78,25 +75,7 @@
         config = keras.saving.serialize_keras_object(self.tokenizer)
         new_tokenizer = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_tokenizer.get_config(),
             self.tokenizer.get_config(),
         )
 
-    @pytest.mark.large  # Saving is slow, so mark these large.
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant([" airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_backbone_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Test for RoBERTa backbone models."""
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
 from keras_nlp.src.tests.test_case import TestCase
@@ -32,16 +33,16 @@
             num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
         )
         self.batch_size = 8
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
 
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_valid_call_roberta(self):
@@ -63,16 +64,16 @@
             keras.saving.serialize_keras_object(self.backbone)
         )
         self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
     def test_variable_sequence_length_call_roberta(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "padding_mask": ops.ones((2, seq_length), dtype="int32"),
+                "token_ids": np.ones((2, seq_length), dtype="int32"),
+                "padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
             output = self.backbone(input_data)
             self.assertAllEqual(
                 ops.shape(output),
                 (2, seq_length, self.backbone.hidden_dim),
             )
 
@@ -101,16 +102,16 @@
                 num_layers=2,
                 num_heads=2,
                 hidden_dim=64,
                 intermediate_dim=128,
                 max_sequence_length=128,
             )
         self.input_batch = {
-            "token_ids": ops.ones((8, 128), dtype="int32"),
-            "padding_mask": ops.ones((8, 128), dtype="int32"),
+            "token_ids": np.ones((8, 128), dtype="int32"),
+            "padding_mask": np.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_classifier.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_classifier_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_classifier_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for RoBERTa classification model."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
 from keras_nlp.src.models.roberta.roberta_classifier import RobertaClassifier
@@ -74,15 +75,15 @@
         # Setup data.
         self.raw_batch = [
             " airplane at airport",
             " the airplane is the best",
         ]
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, ops.ones((2,)))
+            (self.raw_batch, np.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
     def test_classifier_predict(self):
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,16 +49,20 @@
         merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
         merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
         merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
         merges += ["pla ne"]
         self.merges = merges
         self.preprocessor = RobertaMaskedLMPreprocessor(
             RobertaTokenizer(vocabulary=self.vocab, merges=self.merges),
+            # Simplify our testing by masking every available token.
+            mask_selection_rate=1.0,
+            mask_token_rate=1.0,
+            random_token_rate=0.0,
+            mask_selection_length=5,
             sequence_length=5,
-            mask_selection_length=2,
         )
         self.backbone = RobertaBackbone(
             vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_preprocessor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for RoBERTa preprocessor layer."""
-import os
+"""Tests for BART preprocessor layer."""
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
-from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.models.bart.bart_seq_2_seq_lm_preprocessor import (
+    BartSeq2SeqLMPreprocessor,
+)
+from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-class RobertaPreprocessorTest(TestCase):
+class BartSeq2SeqLMPreprocessorTest(TestCase):
     def setUp(self):
         vocab = {
             "<s>": 0,
             "<pad>": 1,
             "</s>": 2,
             "Ġair": 3,
             "plane": 4,
@@ -43,125 +43,113 @@
         }
 
         merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
         merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
         merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
         merges += ["pla ne"]
 
-        self.preprocessor = RobertaPreprocessor(
-            tokenizer=RobertaTokenizer(
+        self.preprocessor = BartSeq2SeqLMPreprocessor(
+            tokenizer=BartTokenizer(
                 vocabulary=vocab,
                 merges=merges,
             ),
-            sequence_length=12,
+            encoder_sequence_length=10,
+            decoder_sequence_length=9,
         )
 
     def test_tokenize_strings(self):
-        input_data = " airplane at airport"
+        input_data = {
+            "encoder_text": " airplane at airport",
+            "decoder_text": " kohli is the best",
+        }
 
-        output = self.preprocessor(input_data)
+        x_out, y_out, sw_out = self.preprocessor(input_data)
         self.assertAllEqual(
-            output["token_ids"], [0, 3, 4, 5, 3, 6, 2, 1, 1, 1, 1, 1]
+            x_out["encoder_token_ids"], [0, 3, 4, 5, 3, 6, 2, 1, 1, 1]
         )
         self.assertAllEqual(
-            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]
+            x_out["encoder_padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0]
         )
-
-    def test_tokenize_list_of_strings(self):
-        input_data = [" airplane at airport"] * 4
-
-        output = self.preprocessor(input_data)
         self.assertAllEqual(
-            output["token_ids"],
-            [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1, 1, 1]] * 4,
+            x_out["decoder_token_ids"], [2, 0, 7, 8, 9, 10, 11, 2, 1]
         )
-
         self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]] * 4
+            x_out["decoder_padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 0]
         )
+        self.assertAllEqual(y_out, [0, 7, 8, 9, 10, 11, 2, 1, 1])
+        self.assertAllEqual(sw_out, [1, 1, 1, 1, 1, 1, 1, 0, 0])
+
+    def test_tokenize_list_of_strings(self):
+        input_data = {
+            "encoder_text": [" airplane at airport"] * 4,
+            "decoder_text": [" kohli is the best"] * 4,
+        }
 
-    def test_tokenize_labeled_batch(self):
-        x = tf.constant([" airplane at airport"] * 4)
-        y = tf.constant([1] * 4)
-        sw = tf.constant([1.0] * 4)
-        x_out, y_out, sw_out = self.preprocessor(x, y, sw)
+        x_out, y_out, sw_out = self.preprocessor(input_data)
         self.assertAllEqual(
-            x_out["token_ids"], [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1, 1, 1]] * 4
+            x_out["encoder_token_ids"], [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1]] * 4
         )
         self.assertAllEqual(
-            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]] * 4
+            x_out["encoder_padding_mask"],
+            [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0]] * 4,
         )
-        self.assertAllEqual(y_out, y)
-        self.assertAllEqual(sw_out, sw)
-
-    def test_tokenize_labeled_dataset(self):
-        x = tf.constant([" airplane at airport"] * 4)
-        y = tf.constant([1] * 4)
-        sw = tf.constant([1.0] * 4)
-        ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
-        ds = ds.map(self.preprocessor)
-        x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(
-            x_out["token_ids"], [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1, 1, 1]] * 4
+            x_out["decoder_token_ids"], [[2, 0, 7, 8, 9, 10, 11, 2, 1]] * 4
         )
         self.assertAllEqual(
-            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]] * 4
+            x_out["decoder_padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 0]] * 4
         )
-        self.assertAllEqual(y_out, y)
-        self.assertAllEqual(sw_out, sw)
+        self.assertAllEqual(y_out, [[0, 7, 8, 9, 10, 11, 2, 1, 1]] * 4)
+        self.assertAllEqual(sw_out, [[1, 1, 1, 1, 1, 1, 1, 0, 0]] * 4)
 
-    def test_tokenize_multiple_sentences(self):
-        sentence_one = tf.constant(" airplane at airport")
-        sentence_two = tf.constant(" kohli is the best")
+    def test_error_multi_segment_input(self):
+        input_data = {
+            "encoder_text": (
+                tf.constant([" airplane at airport"] * 2),
+                tf.constant([" airplane"] * 2),
+            ),
+            "decoder_text": (
+                tf.constant([" kohli is the best"] * 2),
+                tf.constant([" kohli"] * 2),
+            ),
+        }
+
+        with self.assertRaises(ValueError):
+            self.preprocessor(input_data)
 
-        output = self.preprocessor((sentence_one, sentence_two))
+    def test_generate_preprocess(self):
+        input_data = {
+            "encoder_text": tf.convert_to_tensor([" airplane at airport"]),
+            "decoder_text": tf.convert_to_tensor([" kohli is the best"]),
+        }
+        x_out = self.preprocessor.generate_preprocess(input_data)
         self.assertAllEqual(
-            output["token_ids"], [0, 3, 4, 5, 3, 2, 2, 7, 8, 9, 10, 2]
+            x_out["encoder_token_ids"], [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1]]
         )
         self.assertAllEqual(
-            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
+            x_out["encoder_padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0]]
         )
-
-    def test_tokenize_multiple_batched_sentences(self):
-        sentence_one = tf.constant([" airplane at airport"] * 4)
-        sentence_two = tf.constant([" kohli is the best"] * 4)
-
-        output = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
-            output["token_ids"],
-            [[0, 3, 4, 5, 3, 2, 2, 7, 8, 9, 10, 2]] * 4,
+            x_out["decoder_token_ids"], [[2, 0, 7, 8, 9, 10, 11, 1, 1]]
         )
         self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]] * 4
+            x_out["decoder_padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0, 0]]
         )
 
-    def test_errors_for_2d_list_input(self):
-        ambiguous_input = [["one", "two"], ["three", "four"]]
-        with self.assertRaises(ValueError):
-            self.preprocessor(ambiguous_input)
+    def test_generate_postprocess(self):
+        input_data = {
+            "decoder_token_ids": tf.constant([2, 0, 7, 8, 9, 10, 11, 1, 1]),
+            "decoder_padding_mask": tf.cast(
+                [1, 1, 1, 1, 1, 1, 1, 0, 0], dtype="bool"
+            ),
+        }
+        x = self.preprocessor.generate_postprocess(input_data)
+        self.assertAllEqual(x, " kohli is the best")
 
     def test_serialization(self):
-        config = keras.saving.serialize_keras_object(self.preprocessor)
-        new_preprocessor = keras.saving.deserialize_keras_object(config)
-        self.assertEqual(
-            new_preprocessor.get_config(),
-            self.preprocessor.get_config(),
+        new_preprocessor = keras.saving.deserialize_keras_object(
+            keras.saving.serialize_keras_object(self.preprocessor)
         )
-
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant([" airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
+        self.assertEqual(
+            new_preprocessor.get_config(), self.preprocessor.get_config()
         )
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/roberta/roberta_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/roberta/roberta_tokenizer_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for RoBERTa tokenizer."""
-import os
 
-import pytest
-import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
 class RobertaTokenizerTest(TestCase):
@@ -79,25 +76,7 @@
         config = keras.saving.serialize_keras_object(self.tokenizer)
         new_tokenizer = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_tokenizer.get_config(),
             self.tokenizer.get_config(),
         )
 
-    @pytest.mark.large
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant([" airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_backbone_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,141 +1,162 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for T5 backbone model."""
+"""Test for Whisper backbone models."""
 
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
-from keras_nlp.src.models.t5.t5_backbone import T5Backbone
+from keras_nlp.src.models.whisper.whisper_backbone import WhisperBackbone
 from keras_nlp.src.tests.test_case import TestCase
 
 
 @pytest.mark.tf_only
-class T5Test(TestCase):
+class WhisperBackboneTest(TestCase):
     def setUp(self):
-        self.backbone = T5Backbone(
-            vocabulary_size=4,
+        self.backbone = WhisperBackbone(
+            vocabulary_size=10,
             num_layers=2,
             num_heads=2,
-            hidden_dim=4,
+            hidden_dim=2,
             intermediate_dim=4,
+            max_encoder_sequence_length=6,
+            max_decoder_sequence_length=6,
         )
-        self.batch_size = 2
-        seq_length = 3
         self.input_batch = {
-            "encoder_token_ids": ops.ones(
-                (self.batch_size, seq_length), dtype="int32"
-            ),
-            "encoder_padding_mask": ops.ones(
-                (self.batch_size, seq_length), dtype="int32"
-            ),
-            "decoder_token_ids": ops.ones(
-                (self.batch_size, seq_length), dtype="int32"
-            ),
-            "decoder_padding_mask": ops.ones(
-                (self.batch_size, seq_length), dtype="int32"
-            ),
+            "encoder_features": np.ones((2, 5, 80), dtype="float32"),
+            "decoder_token_ids": np.ones((2, 5), dtype="int32"),
+            "decoder_padding_mask": np.ones((2, 5), dtype="int32"),
         }
+
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
-    def test_valid_call_t5(self):
+    def test_valid_call_whisper(self):
         self.backbone(self.input_batch)
 
     def test_token_embedding(self):
         output = self.backbone.token_embedding(
-            self.input_batch["encoder_token_ids"]
+            self.input_batch["decoder_token_ids"]
         )
-        self.assertEqual(output.shape, (2, 3, 4))
+        self.assertEqual(output.shape, (2, 5, 2))
 
     def test_name(self):
         # Check default name passed through
-        self.assertRegexpMatches(self.backbone.name, "t5_backbone")
+        self.assertRegexpMatches(self.backbone.name, "whisper_backbone")
 
-    def test_variable_sequence_length_call_t5(self):
+    def test_variable_sequence_length_call_whisper(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "encoder_token_ids": ops.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "encoder_padding_mask": ops.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "decoder_token_ids": ops.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "decoder_padding_mask": ops.ones(
-                    (self.batch_size, seq_length), dtype="int32"
+                "encoder_features": np.ones(
+                    (2, seq_length, 80), dtype="float32"
                 ),
+                "decoder_token_ids": np.ones((2, seq_length), dtype="int32"),
+                "decoder_padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
-            outputs = self.backbone(input_data)
-            self.assertIn("encoder_sequence_output", outputs)
-            self.assertIn("decoder_sequence_output", outputs)
+            self.backbone(input_data)
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
     def test_serialization(self):
         new_backbone = keras.saving.deserialize_keras_object(
             keras.saving.serialize_keras_object(self.backbone)
         )
         self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
+    def test_key_projection_bias_absence(self):
+        # Check only for the first encoder layer and first decoder layer.
+        self.assertIsNone(
+            self.backbone.get_layer(
+                "transformer_encoder_layer_0"
+            )._self_attention_layer._key_dense.bias
+        )
+        self.assertIsNone(
+            self.backbone.get_layer(
+                "transformer_decoder_layer_0"
+            )._self_attention_layer._key_dense.bias
+        )
+        self.assertIsNone(
+            self.backbone.get_layer(
+                "transformer_decoder_layer_0"
+            )._cross_attention_layer._key_dense.bias
+        )
+
     @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self):
-        outputs = self.backbone(self.input_batch)
+        model_output = self.backbone(self.input_batch)
         path = os.path.join(self.get_temp_dir(), "model.keras")
         self.backbone.save(path, save_format="keras_v3")
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, T5Backbone)
+        self.assertIsInstance(restored_model, WhisperBackbone)
 
         # Check that output matches.
-        restored_outputs = restored_model(self.input_batch)
-        for key in ["encoder_sequence_output", "decoder_sequence_output"]:
-            self.assertAllClose(outputs[key], restored_outputs[key])
+        restored_output = restored_model(self.input_batch)
+        self.assertAllClose(
+            model_output["encoder_sequence_output"],
+            restored_output["encoder_sequence_output"],
+        )
+        self.assertAllClose(
+            model_output["decoder_sequence_output"],
+            restored_output["decoder_sequence_output"],
+        )
 
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
-class T5BackboneTPUTest(TestCase):
+class WhisperBackboneTPUTest(TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
-            self.backbone = T5Backbone(
-                vocabulary_size=4,
+            self.backbone = WhisperBackbone(
+                vocabulary_size=10,
                 num_layers=2,
                 num_heads=2,
-                hidden_dim=4,
+                hidden_dim=2,
                 intermediate_dim=4,
+                max_encoder_sequence_length=6,
+                max_decoder_sequence_length=6,
             )
+
         self.input_batch = {
-            "token_ids": ops.ones((8, 4), dtype="int32"),
-            "padding_mask": ops.ones((8, 4), dtype="int32"),
+            "encoder_features": np.ones(
+                (
+                    8,
+                    self.backbone.max_encoder_sequence_length,
+                    80,
+                ),
+                dtype="int32",
+            ),
+            "decoder_token_ids": np.ones(
+                (8, self.backbone.max_decoder_sequence_length), dtype="int32"
+            ),
+            "decoder_padding_mask": np.ones(
+                (8, self.backbone.max_decoder_sequence_length), dtype="int32"
+            ),
         }
+
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
-        outputs = self.backbone.predict(self.input_dataset)
-        self.assertIn("encoder_sequence_output", outputs)
-        self.assertIn("decoder_sequence_output", outputs)
+        self.backbone.predict(self.input_dataset)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_layer_norm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_layer_norm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_multi_head_attention.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_tokenizer_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for T5 tokenizer."""
 import io
-import os
 
-import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.t5.t5_tokenizer import T5Tokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
@@ -85,25 +83,7 @@
         config = keras.saving.serialize_keras_object(self.tokenizer)
         new_tokenizer = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_tokenizer.get_config(),
             self.tokenizer.get_config(),
         )
 
-    @pytest.mark.large  # Saving is slow, so mark these large.
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/t5/t5_transformer_layer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/t5/t5_transformer_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/task.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Base class for Task models."""
 
 import os
 
 import keras_core
-import rich
 import tensorflow as tf
+from rich import console as rich_console
+from rich import markup
+from rich import table as rich_table
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.utils.keras_utils import print_msg
 from keras_nlp.src.utils.pipeline_model import PipelineModel
 from keras_nlp.src.utils.python_utils import classproperty
 from keras_nlp.src.utils.python_utils import format_docstring
 
@@ -262,46 +264,46 @@
 
         def bold_text(x):
             return f"[bold]{x}[/]"
 
         if self.preprocessor:
             # Create a rich console for printing. Capture for non-interactive logging.
             if print_fn:
-                console = rich.console.Console(
+                console = rich_console.Console(
                     highlight=False, force_terminal=False, color_system=None
                 )
                 console.begin_capture()
             else:
-                console = rich.console.Console(highlight=False)
+                console = rich_console.Console(highlight=False)
 
-            column_1 = rich.table.Column(
+            column_1 = rich_table.Column(
                 "Tokenizer (type)",
                 justify="left",
                 width=int(0.5 * line_length),
             )
-            column_2 = rich.table.Column(
+            column_2 = rich_table.Column(
                 "Vocab #",
                 justify="right",
                 width=int(0.5 * line_length),
             )
-            table = rich.table.Table(
+            table = rich_table.Table(
                 column_1, column_2, width=line_length, show_lines=True
             )
             tokenizer = self.preprocessor.tokenizer
-            tokenizer_name = rich.markup.escape(tokenizer.name)
+            tokenizer_name = markup.escape(tokenizer.name)
             tokenizer_class = highlight_symbol(
-                rich.markup.escape(tokenizer.__class__.__name__)
+                markup.escape(tokenizer.__class__.__name__)
             )
             table.add_row(
                 f"{tokenizer_name} ({tokenizer_class})",
                 highlight_number(f"{tokenizer.vocabulary_size():,}"),
             )
 
             # Print the to the console.
-            preprocessor_name = rich.markup.escape(self.preprocessor.name)
+            preprocessor_name = markup.escape(self.preprocessor.name)
             console.print(bold_text(f'Preprocessor: "{preprocessor_name}"'))
             console.print(table)
 
             # Output captured summary for non-interactive logging.
             if print_fn:
                 print_fn(console.end_capture(), line_break=False)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/task_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/task_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for Whisper audio feature extractor."""
 
-import os
 
-import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.whisper.whisper_audio_feature_extractor import (
     WhisperAudioFeatureExtractor,
 )
 from keras_nlp.src.tests.test_case import TestCase
@@ -74,25 +72,7 @@
             config
         )
         self.assertEqual(
             new_audio_feature_extractor.get_config(),
             self.audio_feature_extractor.get_config(),
         )
 
-    @pytest.mark.large  # Saving is slow, so mark these large.
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        audio_tensor = tf.ones((2, 200), dtype="float32")
-
-        inputs = keras.Input(dtype="float32", shape=(None,))
-        outputs = self.audio_feature_extractor(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(audio_tensor),
-            restored_model(audio_tensor),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_decoder.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_encoder.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/whisper/whisper_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/whisper/whisper_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,119 +7,123 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import io
 
-"""Tests for Whisper preprocessing layers."""
-import os
-
-import pytest
+import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.whisper.whisper_tokenizer import WhisperTokenizer
+from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import (
+    FNetMaskedLMPreprocessor,
+)
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
-class WhisperTokenizerTest(TestCase):
+class FNetMaskedLMPreprocessorTest(TestCase):
     def setUp(self):
-        self.vocab = {
-            "Ġair": 0,
-            "plane": 1,
-            "Ġat": 2,
-            "port": 3,
-            "Ġkoh": 4,
-            "li": 5,
-            "Ġis": 6,
-            "Ġthe": 7,
-            "Ġbest": 8,
-        }
-
-        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
-        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
-        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
-        merges += ["pla ne"]
-        self.merges = merges
-
-        self.special_tokens = {
-            "<|startoftranscript|>": 9,
-            "<|endoftext|>": 10,
-            "<|notimestamps|>": 11,
-            "<|transcribe|>": 12,
-            "<|translate|>": 13,
-        }
-
-        self.language_tokens = {
-            "<|en|>": 14,
-            "<|fr|>": 15,
-        }
-
-        self.tokenizer = WhisperTokenizer(
-            vocabulary=self.vocab,
-            merges=self.merges,
-            special_tokens=self.special_tokens,
-            language_tokens=self.language_tokens,
-        )
-
-    def test_tokenize(self):
-        input_data = " airplane at airport"
-        output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [0, 1, 2, 0, 3])
-
-    def test_tokenize_batch(self):
-        input_data = [" airplane at airport", " kohli is the best"]
-        output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [[0, 1, 2, 0, 3], [4, 5, 6, 7, 8]])
-
-    def test_detokenize(self):
-        input_tokens = [0, 1, 2, 0, 3]
-        output = self.tokenizer.detokenize(input_tokens)
-        self.assertEqual(output, " airplane at airport")
-
-    def test_detokenize_with_special_tokens(self):
-        input_tokens = [9, 14, 12, 11, 0, 1, 2, 0, 3, 10]
-        output = self.tokenizer.detokenize(input_tokens)
-        print(output)
-        self.assertEqual(
-            output,
-            "<|startoftranscript|><|en|><|transcribe|><|notimestamps|> airplane at airport<|endoftext|>",
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the earth is round"]
+        )
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=12,
+            model_type="WORD",
+            pad_id=0,
+            bos_id=1,
+            eos_id=2,
+            unk_id=3,
+            pad_piece="<pad>",
+            unk_piece="<unk>",
+            bos_piece="[CLS]",
+            eos_piece="[SEP]",
+            user_defined_symbols="[MASK]",
+        )
+        self.proto = bytes_io.getvalue()
+
+        self.preprocessor = FNetMaskedLMPreprocessor(
+            tokenizer=FNetTokenizer(proto=self.proto),
+            mask_selection_rate=1.0,
+            mask_token_rate=1.0,
+            random_token_rate=0.0,
+            mask_selection_length=4,
+            sequence_length=12,
+        )
+
+    def test_preprocess_strings(self):
+        input_data = "the quick brown fox"
+
+        x, y, sw = self.preprocessor(input_data)
+        self.assertAllEqual(
+            x["token_ids"], [1, 4, 4, 4, 4, 2, 0, 0, 0, 0, 0, 0]
         )
+        self.assertAllEqual(x["mask_positions"], [1, 2, 3, 4])
+        self.assertAllEqual(y, [5, 10, 6, 8])
+        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0])
 
-    def test_vocabulary_size(self):
-        self.assertEqual(self.tokenizer.vocabulary_size(), 16)
+    def test_preprocess_list_of_strings(self):
+        input_data = ["the quick brown fox"] * 4
 
-    def test_special_tokens(self):
-        self.assertEqual(self.tokenizer.bos_token_id, 9)
-        self.assertEqual(self.tokenizer.eos_token_id, 10)
-        self.assertEqual(self.tokenizer.pad_token_id, 10)
-        self.assertEqual(self.tokenizer.no_timestamps_token_id, 11)
-        self.assertEqual(self.tokenizer.translate_token_id, 13)
-        self.assertEqual(self.tokenizer.transcribe_token_id, 12)
-
-    def test_errors_missing_special_tokens(self):
-        with self.assertRaises(ValueError):
-            WhisperTokenizer(
-                vocabulary=["a", "b", "c"], merges=[], special_tokens={}
-            )
-
-    @pytest.mark.large  # Saving is slow, so mark these large.
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant([" airplane at airport"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
+        x, y, sw = self.preprocessor(input_data)
+        self.assertAllEqual(
+            x["token_ids"], [[1, 4, 4, 4, 4, 2, 0, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4]] * 4)
+        self.assertAllEqual(y, [[5, 10, 6, 8]] * 4)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0]] * 4)
+
+    def test_preprocess_dataset(self):
+        sentences = tf.constant(["the quick brown fox"] * 4)
+        ds = tf.data.Dataset.from_tensor_slices(sentences)
+        ds = ds.map(self.preprocessor)
+        x, y, sw = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(
+            x["token_ids"], [[1, 4, 4, 4, 4, 2, 0, 0, 0, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4]] * 4)
+        self.assertAllEqual(y, [[5, 10, 6, 8]] * 4)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0]] * 4)
+
+    def test_mask_multiple_sentences(self):
+        sentence_one = tf.constant("the quick")
+        sentence_two = tf.constant("brown fox")
 
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
+        x, y, sw = self.preprocessor((sentence_one, sentence_two))
+        self.assertAllEqual(
+            x["token_ids"], [1, 4, 4, 2, 4, 4, 2, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(x["mask_positions"], [1, 2, 4, 5])
+        self.assertAllEqual(y, [5, 10, 6, 8])
+        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0])
+
+    def test_no_masking_zero_rate(self):
+        no_mask_preprocessor = FNetMaskedLMPreprocessor(
+            self.preprocessor.tokenizer,
+            mask_selection_rate=0.0,
+            mask_selection_length=4,
+            sequence_length=12,
+        )
+        input_data = "the quick brown fox"
 
-        restored_model = keras.models.load_model(path)
+        x, y, sw = no_mask_preprocessor(input_data)
         self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
+            x["token_ids"], [1, 5, 10, 6, 8, 2, 0, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0])
+        self.assertAllEqual(y, [0, 0, 0, 0])
+        self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0])
+
+    def test_serialization(self):
+        config = keras.saving.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.saving.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
         )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for XLM-RoBERTa backbone models."""
 import os
 
+import numpy as np
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
 from keras_nlp.src.tests.test_case import TestCase
@@ -31,16 +32,16 @@
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
         )
         self.input_batch = {
-            "token_ids": ops.ones((2, 5), dtype="int32"),
-            "padding_mask": ops.ones((2, 5), dtype="int32"),
+            "token_ids": np.ones((2, 5), dtype="int32"),
+            "padding_mask": np.ones((2, 5), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_valid_call_xlm_roberta(self):
         self.backbone(self.input_batch)
@@ -52,16 +53,16 @@
     def test_name(self):
         # Check default name passed through
         self.assertRegexpMatches(self.backbone.name, "xlm_roberta_backbone")
 
     def test_variable_sequence_length_call_xlm_roberta(self):
         for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": ops.ones((2, seq_length), dtype="int32"),
-                "padding_mask": ops.ones((2, seq_length), dtype="int32"),
+                "token_ids": np.ones((2, seq_length), dtype="int32"),
+                "padding_mask": np.ones((2, seq_length), dtype="int32"),
             }
             output = self.backbone(input_data)
             self.assertAllEqual(
                 ops.shape(output),
                 (2, seq_length, self.backbone.hidden_dim),
             )
 
@@ -100,16 +101,16 @@
                 num_layers=2,
                 num_heads=2,
                 hidden_dim=64,
                 intermediate_dim=128,
                 max_sequence_length=128,
             )
         self.input_batch = {
-            "token_ids": ops.ones((8, 128), dtype="int32"),
-            "padding_mask": ops.ones((8, 128), dtype="int32"),
+            "token_ids": np.ones((8, 128), dtype="int32"),
+            "padding_mask": np.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for XLM-RoBERTa classification model."""
 
 import io
 import os
 
+import numpy as np
 import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
@@ -73,15 +74,15 @@
 
         self.raw_batch = [
             "the quick brown fox.",
             "the slow brown fox.",
         ]
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, ops.ones((2,)))
+            (self.raw_batch, np.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
     def test_classifier_predict(self):
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,16 +55,20 @@
             eos_piece="</s>",
             user_defined_symbols="[MASK]",
         )
         self.proto = bytes_io.getvalue()
 
         self.preprocessor = XLMRobertaMaskedLMPreprocessor(
             XLMRobertaTokenizer(proto=self.proto),
+            # Simplify our testing by masking every available token.
+            mask_selection_rate=1.0,
+            mask_token_rate=1.0,
+            random_token_rate=0.0,
+            mask_selection_length=5,
             sequence_length=5,
-            mask_selection_length=2,
         )
 
         self.backbone = XLMRobertaBackbone(
             vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
 )
 from keras_nlp.src.tests.test_case import TestCase
 
 
 @pytest.mark.large
+@pytest.mark.tf_only  # TODO: jax OOM.
 class XLMRobertaPresetSmokeTest(TestCase):
     """
     A smoke test for XLM-RoBERTa presets we run continuously.
 
     This only tests the smallest weights we have available. Run with:
     `pytest keras_nlp/models/xlm_roberta/xlm_roberta_presets_test.py --run_large`
     """
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for XLM-RoBERTa tokenizer."""
 import io
-import os
 
-import pytest
 import sentencepiece
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
 )
@@ -111,25 +109,7 @@
         config = keras.saving.serialize_keras_object(self.tokenizer)
         new_tokenizer = keras.saving.deserialize_keras_object(config)
         self.assertEqual(
             new_tokenizer.get_config(),
             self.tokenizer.get_config(),
         )
 
-    @pytest.mark.large  # Saving is slow, so mark these large.
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/beam_sampler.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/beam_sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Beam Sampler."""
 
 import tensorflow as tf
-from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
+from keras_nlp.src.backend import ops
 from keras_nlp.src.samplers.sampler import Sampler
 from keras_nlp.src.samplers.sampler import call_args_docstring
 from keras_nlp.src.utils.python_utils import format_docstring
-from keras_nlp.src.utils.tensor_utils import assert_tf_backend
 
 
 @format_docstring(call_args=call_args_docstring)
 @keras_nlp_export("keras_nlp.samplers.BeamSampler")
 class BeamSampler(Sampler):
     """Beam Sampler class.
 
@@ -98,140 +97,145 @@
 
     def __init__(
         self,
         num_beams=5,
         return_all_beams=False,
         **kwargs,
     ):
-        # Temporarily turn off beam search in other backends.
-        # No technical blockers here, just need tf -> ops rewrite.
-        assert_tf_backend(self.__class__.__name__)
-
         super().__init__(**kwargs)
         self.num_beams = num_beams
         self.return_all_beams = return_all_beams
 
     def __call__(
         self,
         next,
         prompt,
         cache=None,
         index=0,
         mask=None,
         end_token_id=None,
         hidden_states=None,
     ):
-        batch_size, max_length = tf.shape(prompt)[0], tf.shape(prompt)[1]
-        # Make sure max length and start index are the same dtype.
-        index = tf.cast(index, max_length.dtype)
+        batch_size, max_length = ops.shape(prompt)[0], ops.shape(prompt)[1]
+        index = ops.cast(index, "int32")
 
         def create_beams(x):
             """Add initial beam state."""
-            return tf.repeat(x, self.num_beams, axis=0)
+            return ops.repeat(x, self.num_beams, axis=0)
 
         def flatten_beams(x):
             """Combine the beam dim and batch dim."""
-            flat_shape = [batch_size * self.num_beams] + x.shape.as_list()[2:]
-            return tf.reshape(x, shape=flat_shape)
+            flat_shape = (batch_size * self.num_beams,) + tuple(x.shape)[2:]
+            return ops.reshape(x, flat_shape)
 
         def unflatten_beams(x):
             """Separate the beam dim and batch dim."""
-            unflat_shape = [batch_size, self.num_beams] + x.shape.as_list()[1:]
-            return tf.reshape(x, shape=unflat_shape)
+            unflat_shape = (batch_size, self.num_beams) + tuple(x.shape)[1:]
+            return ops.reshape(x, unflat_shape)
 
         if mask is None:
-            mask = tf.zeros_like(prompt, dtype="bool")
+            mask = ops.zeros_like(prompt, dtype="bool")
         else:
-            mask = tf.cast(mask, dtype="bool")
-        # `tf.while_loop` will not accept `None` as a value for `loop_vars`.
-        cache = () if cache is None else cache
+            mask = ops.cast(mask, dtype="bool")
+        # `ops.while_loop` will not accept `None` as a value for `loop_vars`.
+        has_cache = cache is not None
+        cache = cache if has_cache else ()
         # Add extra sequences for each beam.
         prompt, mask = create_beams(prompt), create_beams(mask)
         cache = tf.nest.map_structure(create_beams, cache)
         # Setup the initial beam log-likelihoods.
         # On the first loop, make sure only the original beam is considered.
-        log_probs = tf.constant([[0.0] + [-1e9] * (self.num_beams - 1)])
-        log_probs = flatten_beams(tf.repeat(log_probs, batch_size, axis=0))
+        log_probs = ops.array(
+            [[0.0] + [-1e9] * (self.num_beams - 1)], dtype="float32"
+        )
+        log_probs = flatten_beams(ops.repeat(log_probs, batch_size, axis=0))
 
         def cond(prompt, cache, index, log_probs):
             if end_token_id is None:
                 return True
             # Stop if all sequences have produced a *new* end_token_id.
             end_tokens = (prompt == end_token_id) & (~mask)
-            prompt_done = tf.reduce_any(end_tokens, axis=-1)
-            return not tf.reduce_all(prompt_done)
+            prompt_done = ops.any(end_tokens, axis=-1)
+            return ops.logical_not(ops.all(prompt_done))
 
         def body(prompt, cache, index, log_probs):
             # Compute the softmax distribution for the next token.
             logits, _, cache = next(prompt, cache, index)
-            vocab_size = tf.shape(logits)[-1]
+            vocab_size = ops.shape(logits)[-1]
             probs = keras.activations.softmax(logits / self.temperature)
 
             # Compute the running log-likelihood of each new candidate.
-            next_log_probs = tf.math.log(probs) + log_probs[..., tf.newaxis]
+            next_log_probs = ops.log(probs) + log_probs[..., None]
             # Reshape `preds` to shape `(batch_size, num_beams * vocab_size)`.
-            next_log_probs = tf.reshape(next_log_probs, shape=[batch_size, -1])
+            next_log_probs = ops.reshape(next_log_probs, [batch_size, -1])
 
             # Compute the top beam indices and next tokens.
-            next_log_probs, indices = tf.math.top_k(
+            next_log_probs, indices = ops.top_k(
                 next_log_probs, k=self.num_beams, sorted=False
             )
             beam_indices = indices // vocab_size
             next_token = flatten_beams(indices % vocab_size)
-            # Ensure shape is `[None]`, otherwise it causes issues after
-            # converting to TFLite.
-            next_token = tf.ensure_shape(next_token, [None])
             # We need `ensure_shape` as `top_k` will change the static shape.
             next_log_probs = flatten_beams(next_log_probs)
-            log_probs = tf.ensure_shape(next_log_probs, log_probs.shape)
+            # Work around for top_k output shape on tf backend.
+            if isinstance(log_probs, tf.Tensor):
+                log_probs = tf.ensure_shape(next_log_probs, log_probs.shape)
+            else:
+                log_probs = next_log_probs
 
             def gather_beams(x):
                 x = unflatten_beams(x)
-                x = tf.gather(x, beam_indices, axis=1, batch_dims=1)
+                indices = beam_indices
+                for axis in range(2, len(x.shape)):
+                    indices = ops.expand_dims(indices, axis=axis)
+                x = ops.take_along_axis(x, indices, axis=1)
                 return flatten_beams(x)
 
             prompt = gather_beams(prompt)
-            cache = tf.nest.map_structure(gather_beams, cache)
+            if has_cache:
+                cache = tf.nest.map_structure(gather_beams, cache)
 
             # Update each beam with the next token.
-            next_token = tf.cast(next_token, prompt.dtype)
+            next_token = ops.cast(next_token, prompt.dtype)
             # Don't overwrite anywhere mask is True.
-            next_token = tf.where(mask[:, index], prompt[:, index], next_token)
+            next_token = ops.where(mask[:, index], prompt[:, index], next_token)
             # Update the prompt with the next token.
-            next_token = next_token[:, tf.newaxis]
-            prompt = dynamic_update_slice(prompt, next_token, [0, index])
+            next_token = next_token[:, None]
+            prompt = ops.slice_update(prompt, [0, index], next_token)
             # Return the iteration of the loop state.
             return (prompt, cache, index + 1, log_probs)
 
-        prompt, _, _, log_probs = tf.while_loop(
+        prompt, _, _, log_probs = self.run_loop(
             cond=cond,
             body=body,
             loop_vars=(prompt, cache, index, log_probs),
             maximum_iterations=(max_length - index),
         )
 
         all_prompts = unflatten_beams(prompt)
         all_log_probs = unflatten_beams(log_probs)
 
         if self.return_all_beams:
-            sorted_indices = tf.argsort(
-                all_log_probs, axis=-1, direction="DESCENDING"
-            )
-            sorted_log_probs = tf.gather(
-                all_log_probs, sorted_indices, axis=-1, batch_dims=1
+            sorted_indices = ops.argsort(-all_log_probs, axis=-1)
+            sorted_log_probs = ops.take_along_axis(
+                all_log_probs,
+                sorted_indices,
+                axis=1,
             )
-            sorted_prompts = tf.gather(
-                all_prompts, sorted_indices, axis=1, batch_dims=1
+            sorted_prompts = ops.take_along_axis(
+                all_prompts,
+                ops.expand_dims(sorted_indices, -1),
+                axis=1,
             )
             return sorted_prompts, sorted_log_probs
         else:
             # Gather the top beam at each batch index.
-            top_beams = tf.math.argmax(all_log_probs, axis=-1)[:, tf.newaxis]
-            prompt = tf.gather(all_prompts, top_beams, axis=1, batch_dims=1)
-            return tf.squeeze(prompt, axis=1)
+            top_beams = ops.argmax(all_log_probs, axis=-1)[:, None, None]
+            prompt = ops.take_along_axis(all_prompts, top_beams, axis=1)
+            return ops.squeeze(prompt, axis=1)
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_beams": self.num_beams,
                 "return_all_beams": self.return_all_beams,
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/beam_sampler_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/beam_sampler_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from absl.testing import parameterized
 
 from keras_nlp.src.backend import ops
 from keras_nlp.src.samplers.beam_sampler import BeamSampler
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
 class BeamSamplerTest(TestCase):
     def setUp(self):
         super().setUp()
         # Use a simple alphabet of lowercase characters to [0, 26).
         self.int_lookup = {i: chr(i + ord("a")) for i in range(26)}
         self.char_lookup = {v: k for k, v in self.int_lookup.items()}
         self.batch_size = 1
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/contrastive_sampler.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/contrastive_sampler.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Contrastive Sampler."""
 
 import tensorflow as tf
-from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
+from keras_nlp.src.backend import ops
 from keras_nlp.src.samplers.sampler import Sampler
 from keras_nlp.src.samplers.sampler import call_args_docstring
 from keras_nlp.src.utils.python_utils import format_docstring
-from keras_nlp.src.utils.tensor_utils import assert_tf_backend
 
 
 @format_docstring(call_args=call_args_docstring)
 @keras_nlp_export("keras_nlp.samplers.ContrastiveSampler")
 class ContrastiveSampler(Sampler):
     """Contrastive Sampler class.
 
@@ -75,18 +74,14 @@
     def __init__(
         self,
         k=5,
         alpha=0.6,
         seed=None,
         **kwargs,
     ):
-        # Temporarily turn off beam search in other backends.
-        # No technical blockers here, just need tf -> ops rewrite.
-        assert_tf_backend(self.__class__.__name__)
-
         super().__init__(**kwargs)
         self.k = k
         self.alpha = alpha
         self.seed = seed
 
     def __call__(
         self,
@@ -99,147 +94,152 @@
         hidden_states=None,
     ):
         if hidden_states is None:
             raise ValueError(
                 "`ContrastiveSampler` requires passing a `hidden_states`, but"
                 "received `None`."
             )
-        batch_size, max_length = tf.shape(prompt)[0], tf.shape(prompt)[1]
-        # Make sure max length and start index are the same dtype.
-        index = tf.cast(index, max_length.dtype)
+        batch_size, max_length = ops.shape(prompt)[0], ops.shape(prompt)[1]
+        index = ops.cast(index, "int32")
 
         def create_beams(x):
             """Add initial beam state."""
-            x = tf.repeat(x, self.k, axis=0)
-            flat_shape = [batch_size * self.k] + x.shape.as_list()[1:]
-            return tf.reshape(x, shape=flat_shape)
+            x = ops.repeat(x, self.k, axis=0)
+            flat_shape = (batch_size * self.k,) + tuple(x.shape)[1:]
+            return ops.reshape(x, flat_shape)
 
         def flatten_beams(x):
             """Combine the beam dim and batch dim."""
-            flat_shape = [batch_size * self.k] + x.shape.as_list()[2:]
-            return tf.reshape(x, shape=flat_shape)
+            flat_shape = (batch_size * self.k,) + tuple(x.shape)[2:]
+            return ops.reshape(x, flat_shape)
 
         def unflatten_beams(x):
             """Separate the beam dim and batch dim."""
-            unflat_shape = [batch_size, self.k] + x.shape.as_list()[1:]
-            return tf.reshape(x, shape=unflat_shape)
+            unflat_shape = (batch_size, self.k) + tuple(x.shape)[1:]
+            return ops.reshape(x, unflat_shape)
 
-        mask = tf.zeros_like(prompt, dtype="bool") if mask is None else mask
+        mask = ops.zeros_like(prompt, dtype="bool") if mask is None else mask
         # Compute initial logits.
         logits, _, cache = next(prompt, cache, index)
-        # `tf.while_loop` will not accept `None` as a value for `loop_vars`.
-        cache = () if cache is None else cache
+        # `ops.while_loop` will not accept `None` as a value for `loop_vars`.
+        has_cache = cache is not None
+        cache = cache if has_cache else ()
 
         def cond(prompt, cache, index, logits, hidden_states):
             if end_token_id is None:
                 return True
             # Stop if all sequences have produced a *new* end_token_id.
             end_tokens = (prompt == end_token_id) & (~mask)
-            prompt_done = tf.reduce_any(end_tokens, axis=-1)
-            return not tf.reduce_all(prompt_done)
+            prompt_done = ops.any(end_tokens, axis=-1)
+            return ops.logical_not(ops.all(prompt_done))
 
         def body(prompt, cache, index, logits, hidden_states):
             # Compute the softmax distribution for the next token.
             probabilities = keras.activations.softmax(logits / self.temperature)
 
             # Replicate for `self.k` times to find the best token in top-k
             # candidates.
             prompt_beams = create_beams(prompt)
             mask_beams = create_beams(mask)
             hidden_states_beams = create_beams(hidden_states)
-            cache_beams = tf.nest.map_structure(create_beams, cache)
+            cache_beams = None
+            if has_cache:
+                cache_beams = tf.nest.map_structure(create_beams, cache)
 
             # Get top-k candidate tokens and their probabilities.
-            top_k_probabilities, top_k_indices = tf.math.top_k(
+            top_k_probabilities, top_k_indices = ops.top_k(
                 probabilities, k=self.k, sorted=False
             )
             next_token_probabilities = flatten_beams(top_k_probabilities)
             next_token = flatten_beams(top_k_indices)
-            next_token = tf.cast(next_token, prompt.dtype)
-            next_token = tf.where(
+            next_token = ops.cast(next_token, prompt.dtype)
+            next_token = ops.where(
                 mask_beams[:, index], prompt_beams[:, index], next_token
             )
 
             # Update the prompt with the next token.
-            next_token = next_token[:, tf.newaxis]
-            prompt_beams = dynamic_update_slice(
-                prompt_beams, next_token, [0, index]
+            next_token = ops.expand_dims(next_token, -1)
+            prompt_beams = ops.slice_update(
+                prompt_beams, [0, index], next_token
             )
 
             # Compute the logits and hidden states for top-k candidate tokens.
             next_logits, next_hidden_states_beams, cache_beams = next(
                 prompt_beams, cache_beams, index + 1
             )
 
             # Compute the max similarity score for top-k candidate tokens
             # against previous tokens.
             similarity_scores = self.similarity(
                 hidden_states_beams, next_hidden_states_beams
             )
-            max_similarity_scores = tf.cast(
-                tf.reduce_max(similarity_scores[:, :index], axis=1),
+            # Replace all future indices with -1, the lowest similarity score.
+            score_mask = ops.expand_dims(ops.arange(max_length) < index, 0)
+            similarity_scores = ops.where(score_mask, similarity_scores, -1)
+            max_similarity_scores = ops.cast(
+                ops.max(similarity_scores, axis=1),
                 dtype=next_token_probabilities.dtype,
             )
-            if index == 0:
-                # If the index is 0, there is no previous states so we set
-                # `max_similarity_scores` the same for all beams.
-                max_similarity_scores = tf.zeros_like(max_similarity_scores)
             # The final score of each candidate token is weighted sum of
             # probability and similarity against previous tokens.
             accumulated_scores = (
                 (1 - self.alpha) * next_token_probabilities
                 - self.alpha * max_similarity_scores
             )
             # Unflatten varibles to shape [batch_size, self.k, ...] for
             # gather purpose.
             unflat_score = unflatten_beams(accumulated_scores)
             unflat_prompt = unflatten_beams(prompt_beams)
             unflat_next_logits = unflatten_beams(next_logits)
             unflat_next_hidden_states = unflatten_beams(
                 next_hidden_states_beams
             )
-            unflat_cache = tf.nest.map_structure(unflatten_beams, cache_beams)
-            best_token_indices = tf.math.argmax(unflat_score, axis=1)
+            best_token_indices = ops.argmax(unflat_score, axis=1)
 
             def gather_best_token(beams):
-                return tf.gather(
+                indices = best_token_indices
+                for axis in range(1, len(beams.shape)):
+                    indices = ops.expand_dims(indices, axis=axis)
+                best = ops.take_along_axis(
                     beams,
-                    best_token_indices,
+                    indices,
                     axis=1,
-                    batch_dims=1,
                 )
+                return ops.squeeze(best, axis=1)
 
             prompt = gather_best_token(unflat_prompt)
             # We avoid recomputing forward pass for each token by updating the
             # cache/hidden_states using the output, and pass the logits to
             # next iteration step.
             logits = gather_best_token(unflat_next_logits)
             next_hidden_states = gather_best_token(unflat_next_hidden_states)
-            cache = tf.nest.map_structure(gather_best_token, unflat_cache)
+            if has_cache:
+                cache = tf.nest.map_structure(unflatten_beams, cache_beams)
+                cache = tf.nest.map_structure(gather_best_token, cache)
 
-            hidden_states = dynamic_update_slice(
+            hidden_states = ops.slice_update(
                 hidden_states,
-                next_hidden_states[:, tf.newaxis, :],
                 [0, index, 0],
+                next_hidden_states[:, None, :],
             )
             return (prompt, cache, index + 1, logits, hidden_states)
 
-        prompt, _, _, _, _ = tf.while_loop(
+        prompt, _, _, _, _ = self.run_loop(
             cond=cond,
             body=body,
             loop_vars=(prompt, cache, index, logits, hidden_states),
             maximum_iterations=(max_length - index),
         )
         return prompt
 
     def similarity(self, h1, h2):
-        h2 = h2[..., tf.newaxis]
-        return tf.squeeze(tf.matmul(h1, h2), axis=-1) / (
-            tf.norm(h1, axis=-1) * tf.norm(h2, axis=-2)
-        )
+        h2 = ops.expand_dims(h2, -1)
+        h1_norm = ops.sqrt(ops.sum(h1 * h1, axis=-1))
+        h2_norm = ops.sqrt(ops.sum(h2 * h2, axis=-2))
+        return ops.squeeze(ops.matmul(h1, h2), axis=-1) / (h1_norm * h2_norm)
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "k": self.k,
                 "alpha": self.alpha,
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/contrastive_sampler_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/contrastive_sampler_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from absl.testing import parameterized
 
 from keras_nlp.src.backend import ops
 from keras_nlp.src.samplers.contrastive_sampler import ContrastiveSampler
 from keras_nlp.src.tests.test_case import TestCase
 
 
-@pytest.mark.tf_only
 class ContrastiveSamplerTest(TestCase):
     def setUp(self):
         super().setUp()
         # Use a simple alphabet of lowercase characters to [0, 26).
         self.int_lookup = {i: chr(i + ord("a")) for i in range(26)}
         self.char_lookup = {v: k for k, v in self.int_lookup.items()}
         self.batch_size = 1
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/greedy_sampler.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/greedy_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/greedy_sampler_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/greedy_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/random_sampler.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/random_sampler_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/random_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/sampler.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/serialization.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/serialization_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/serialization_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/top_k_sampler.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/top_k_sampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,15 +76,17 @@
         top_k_pred, top_k_indices = ops.top_k(
             probabilities,
             k=self.k,
             sorted=False,
         )
         # Sample the next token from the probability distribution.
         sample_indices = random.categorical(
-            ops.log(top_k_pred),
+            # tf does not support half precision multinomial sampling, so make
+            # sure we have full precision here.
+            ops.cast(ops.log(top_k_pred), "float32"),
             1,
             seed=self.seed_generator,
             dtype="int32",
         )
 
         # Rearrange to get the next token idx from the original order.
         output = ops.take_along_axis(top_k_indices, sample_indices, axis=-1)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/top_k_sampler_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/top_k_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/top_p_sampler.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/top_p_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/samplers/top_p_sampler_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/samplers/top_p_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tests/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tests/doc_tests/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tests/doc_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tests/doc_tests/docstring_lib.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tests/doc_tests/docstring_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tests/doc_tests/docstring_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tests/doc_tests/docstring_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tests/test_case.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tests/test_case.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,42 +13,44 @@
 # limitations under the License.
 import tensorflow as tf
 from absl.testing import parameterized
 
 from keras_nlp.src.backend import ops
 
 
-class TestCase(tf.test.TestCase, parameterized.TestCase):
-    """Base test case class for KerasNLP.
+def convert_to_comparible_type(x):
+    """Convert tensors to comparable types.
 
-    For now we just extend tf.TestCase and parameterized.TestCase, but this
-    indirection will allow us to add more functionality in the future if we
-    want.
+    Any string are converted to plain python types. Any jax or torch tensors
+    are converted to numpy.
     """
+    if getattr(x, "dtype", None) == tf.string:
+        if isinstance(x, tf.RaggedTensor):
+            x = x.to_list()
+        if isinstance(x, tf.Tensor):
+            x = x.numpy() if x.shape.rank == 0 else x.numpy().tolist()
+        return tf.nest.map_structure(lambda x: x.decode("utf-8"), x)
+    if isinstance(x, (tf.Tensor, tf.RaggedTensor)):
+        return x
+    if ops.is_tensor(x):
+        return ops.convert_to_numpy(x)
+    return x
 
-    def assertAllClose(self, x1, x2, atol=1e-6, rtol=1e-6, msg=None):
-        def convert_to_numpy(x):
-            return ops.convert_to_numpy(x) if ops.is_tensor(x) else x
 
-        x1 = tf.nest.map_structure(convert_to_numpy, x1)
-        x2 = tf.nest.map_structure(convert_to_numpy, x2)
-        super().assertAllClose(x1, x2, atol=atol, rtol=rtol, msg=msg)
+class TestCase(tf.test.TestCase, parameterized.TestCase):
+    """Base test case class for KerasNLP."""
 
-    def assertAllEqual(self, x1, x2, msg=None):
-        def convert_strings(x):
-            """Convert any string tensors to simple python types.
+    def assertAllClose(self, x1, x2, atol=1e-6, rtol=1e-6, msg=None):
+        x1 = tf.nest.map_structure(convert_to_comparible_type, x1)
+        x2 = tf.nest.map_structure(convert_to_comparible_type, x2)
+        super().assertAllClose(x1, x2, atol=atol, rtol=rtol, msg=msg)
 
-            This allows for simple output comparisons across backends without
-            needing to worry about tensorflow's bytes representation.
-            """
-            if getattr(x, "dtype", None) == tf.string:
-                if isinstance(x, tf.RaggedTensor):
-                    x = x.to_list()
-                if isinstance(x, tf.Tensor):
-                    x = x.numpy() if x.shape.rank == 0 else x.numpy().tolist()
-                return tf.nest.map_structure(lambda x: x.decode("utf-8"), x)
-            return x
+    def assertEqual(self, x1, x2, msg=None):
+        x1 = tf.nest.map_structure(convert_to_comparible_type, x1)
+        x2 = tf.nest.map_structure(convert_to_comparible_type, x2)
+        super().assertEqual(x1, x2, msg=msg)
 
-        x1 = tf.nest.map_structure(convert_strings, x1)
-        x2 = tf.nest.map_structure(convert_strings, x2)
+    def assertAllEqual(self, x1, x2, msg=None):
+        x1 = tf.nest.map_structure(convert_to_comparible_type, x1)
+        x2 = tf.nest.map_structure(convert_to_comparible_type, x2)
         super().assertAllEqual(x1, x2, msg=msg)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.tests.test_case import TestCase
 from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
@@ -167,22 +166,7 @@
             self.tokenizer.get_config()
         )
         self.assertAllEqual(
             self.tokenizer(input_data),
             cloned_tokenizer(input_data),
         )
 
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["the quick brown whale."])
-        tokenizer = self.tokenizer
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/byte_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/byte_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/byte_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/byte_tokenizer_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 
-import pytest
 import tensorflow as tf
 
-from keras_nlp.src.backend import keras
 from keras_nlp.src.tests.test_case import TestCase
 from keras_nlp.src.tokenizers.byte_tokenizer import ByteTokenizer
 
 
 class ByteTokenizerTest(TestCase):
     def test_tokenize(self):
         input_data = ["hello", "fun", "▀▁▂▃"]
@@ -178,24 +175,14 @@
             [104, 101, 108, 108, 111, 0, 0, 0, 0, 0],
             [102, 117, 110, 0, 0, 0, 0, 0, 0, 0],
             [226, 150, 128, 226, 150, 129, 226, 150, 130, 226],
             [104, 97, 104, 97, 0, 0, 0, 0, 0, 0],
         ]
         self.assertAllEqual(output, exp_output)
 
-    @pytest.mark.tf_only
-    def test_functional_model(self):
-        input_data = tf.constant(["hello", "fun", "▀▁▂▃"])
-        tokenizer = ByteTokenizer()
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer.detokenize(tokenizer.tokenize(inputs))
-        model = keras.Model(inputs, outputs)
-        model_output = model(input_data)
-        self.assertAllEqual(model_output, ["hello", "fun", "▀▁▂▃"])
-
     def test_load_model_with_config(self):
         input_data = ["hello"]
 
         original_tokenizer = ByteTokenizer(
             lowercase=False,
             sequence_length=8,
             normalization_form="NFC",
@@ -232,29 +219,7 @@
             "normalization_form": "NFC",
             "replacement_char": 0,
             "sequence_length": 8,
             "trainable": True,
         }
         self.assertEqual(tokenizer.get_config(), exp_config)
 
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["this is fun"])
-
-        tokenizer = ByteTokenizer(
-            name="byte_tokenizer_config_test",
-            lowercase=False,
-            sequence_length=20,
-            normalization_form="NFKC",
-            errors="replace",
-        )
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import os
 
-import pytest
 import sentencepiece
 import tensorflow as tf
 
-from keras_nlp.src.backend import keras
 from keras_nlp.src.tests.test_case import TestCase
 from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
 
 
 class SentencePieceTokenizerTest(TestCase):
     def setUp(self):
         super().setUp()
@@ -110,26 +108,14 @@
             proto=self.proto,
         )
         with self.assertRaises(ValueError):
             tokenizer.id_to_token(tokenizer.vocabulary_size())
         with self.assertRaises(ValueError):
             tokenizer.id_to_token(-1)
 
-    @pytest.mark.tf_only
-    def test_functional_model(self):
-        input_data = tf.constant(["the quick brown fox."])
-        tokenizer = SentencePieceTokenizer(
-            proto=self.proto,
-        )
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer.detokenize(tokenizer.tokenize(inputs))
-        model = keras.Model(inputs, outputs)
-        model_output = model(input_data)
-        self.assertAllEqual(model_output, ["the quick brown fox."])
-
     def test_from_file(self):
         filepath = os.path.join(self.get_temp_dir(), "model.txt")
         input_data = ["the quick brown fox."]
         with tf.io.gfile.GFile(filepath, "wb") as file:
             file.write(self.proto)
         tokenizer = SentencePieceTokenizer(
             proto=filepath,
@@ -188,27 +174,7 @@
             original_tokenizer.get_config()
         )
         self.assertAllEqual(
             original_tokenizer(input_data),
             cloned_tokenizer(input_data),
         )
 
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        filepath = os.path.join(self.get_temp_dir(), "model.txt")
-        input_data = tf.constant(["the quick brown whale."])
-        with tf.io.gfile.GFile(filepath, "wb") as file:
-            file.write(self.proto)
-        tokenizer = SentencePieceTokenizer(
-            proto=filepath,
-        )
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,24 +62,14 @@
     tokenizer.detokenize(["This", "is", "a", "test"])
     ```
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def __new__(cls, *args, **kwargs):
-        # Wrap the `tokenize` and `detokenize` methods so they route through
-        # __call__. This is needed for functional model support.
-        obj = super().__new__(cls, *args, **kwargs)
-        obj._tokenize_without_call = obj.tokenize
-        obj._detokenize_without_call = obj.detokenize
-        obj.tokenize = obj._tokenize_with_call
-        obj.detokenize = obj._detokenize_with_call
-        return obj
-
     def tokenize(self, inputs, *args, **kwargs):
         """Transform input tensors of strings into output tokens.
 
         Args:
             inputs: Input tensor, or dict/list/tuple of input tensors.
             *args: Additional positional arguments.
             **kwargs: Additional keyword arguments.
@@ -127,23 +117,13 @@
     def token_to_id(self, token: str) -> int:
         """Convert an integer id to a string token."""
         raise NotImplementedError(
             "No implementation of `id_to_token()` was found for "
             f"{self.__class__.__name__}."
         )
 
-    def _tokenize_with_call(self, *args, **kwargs):
-        return self(*args, mode="tokenize", **kwargs)
-
-    def _detokenize_with_call(self, *args, **kwargs):
-        return self(*args, mode="detokenize", **kwargs)
+    def call(self, inputs, *args, training=None, **kwargs):
+        return self.tokenize(inputs, *args, **kwargs)
 
-    def call(self, *args, mode="tokenize", training=None, **kwargs):
-        if mode == "tokenize":
-            return self._tokenize_without_call(*args, **kwargs)
-        elif mode == "detokenize":
-            return self._detokenize_without_call(*args, **kwargs)
-        else:
-            raise ValueError(
-                f"Unsupported tokenizer mode. Received: mode={mode}"
-            )
+    def compute_output_shape(self, inputs_shape):
+        return tuple(inputs_shape) + (self.sequence_length,)
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/tokenizer_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
 import tensorflow as tf
 
-from keras_nlp.src.backend import keras
 from keras_nlp.src.tests.test_case import TestCase
 from keras_nlp.src.tokenizers.tokenizer import Tokenizer
 
 
 class SimpleTokenizer(Tokenizer):
     __test__ = False  # for pytest
 
@@ -41,23 +39,11 @@
 
     def test_detokenize(self):
         input_data = ["the", "quick", "brown", "fox"]
         tokenizer = SimpleTokenizer()
         detokenize_output = tokenizer.detokenize(input_data)
         self.assertAllEqual(detokenize_output, ["the quick brown fox"])
 
-    @pytest.mark.tf_only
-    def test_functional_model(self):
-        input_data = tf.constant(["the   quick   brown   fox"])
-        tokenizer = SimpleTokenizer()
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer.detokenize(tokenizer.tokenize(inputs))
-        model = keras.Model(inputs, outputs)
-        model_output = model(input_data)
-        # There appears to be a bug with shape inference for ragged reduce_join.
-        # The second dimension should be removed.
-        self.assertAllEqual(model_output, [["the quick brown fox"]])
-
     def test_missing_tokenize_raises(self):
         with self.assertRaises(NotImplementedError):
             Tokenizer()(["the quick brown fox"])
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 
-import pytest
 import tensorflow as tf
 
-from keras_nlp.src.backend import keras
 from keras_nlp.src.tests.test_case import TestCase
 from keras_nlp.src.tokenizers.unicode_codepoint_tokenizer import (
     UnicodeCodepointTokenizer,
 )
 
 
 class UnicodeCodepointTokenizerTest(TestCase):
@@ -232,35 +229,14 @@
             [115, 97, 109, 117, 114, 97, 105, 0, 0, 0],
             [9600, 9601, 9602, 9603, 0, 0, 0, 0, 0, 0],
             [107, 101, 114, 97, 115, 0, 0, 0, 0, 0],
             [116, 101, 110, 115, 111, 114, 102, 108, 111, 119],
         ]
         self.assertAllEqual(output, exp_output)
 
-    @pytest.mark.tf_only
-    def test_functional_model(self):
-        input_data = tf.constant(
-            ["ninja", "samurai", "▀▁▂▃", "keras", "tensorflow"]
-        )
-        tokenizer = UnicodeCodepointTokenizer()
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer.detokenize(tokenizer.tokenize(inputs))
-        model = keras.Model(inputs, outputs)
-        model_output = model(input_data)
-        self.assertAllEqual(
-            model_output,
-            [
-                b"ninja",
-                b"samurai",
-                b"\xe2\x96\x80\xe2\x96\x81\xe2\x96\x82\xe2\x96\x83",
-                b"keras",
-                b"tensorflow",
-            ],
-        )
-
     def test_load_model_with_config(self):
         input_data = tf.constant(["hello"])
 
         original_tokenizer = UnicodeCodepointTokenizer(
             lowercase=False,
             sequence_length=11,
             normalization_form="NFC",
@@ -330,30 +306,7 @@
             "vocabulary_size": None,
         }
         self.assertEqual(
             tokenize_different_encoding.get_config(),
             exp_config_different_encoding,
         )
 
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["ninjas and samurais", "time travel"])
-
-        tokenizer = UnicodeCodepointTokenizer(
-            name="unicode_character_tokenizer_config_gen",
-            lowercase=False,
-            sequence_length=20,
-            normalization_form="NFKC",
-            errors="replace",
-            vocabulary_size=None,
-        )
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
-import pytest
 import tensorflow as tf
 
-from keras_nlp.src.backend import keras
 from keras_nlp.src.tests.test_case import TestCase
 from keras_nlp.src.tokenizers.word_piece_tokenizer import WordPieceTokenizer
 
 
 class WordPieceTokenizerTest(TestCase):
     def test_tokenize(self):
         input_data = ["the quick brown fox."]
@@ -152,25 +150,14 @@
             lowercase=False,
             strip_accents=False,
             split=False,
         )
         call_output = tokenizer(input_data)
         self.assertAllEqual(call_output, [1, 2, 3, 4, 5, 6])
 
-    @pytest.mark.tf_only
-    def test_functional_model(self):
-        input_data = tf.constant(["the quick brown fox"])
-        vocab_data = ["[UNK]", "the", "qu", "##ick", "br", "##own", "fox"]
-        tokenizer = WordPieceTokenizer(vocabulary=vocab_data)
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer.detokenize(tokenizer.tokenize(inputs))
-        model = keras.Model(inputs, outputs)
-        model_output = model(input_data)
-        self.assertAllEqual(model_output, ["the quick brown fox"])
-
     def test_batching_ragged_tensors(self):
         tokenizer = WordPieceTokenizer(
             vocabulary=["[UNK]", "a", "b", "c", "d", "e", "f"]
         )
         dataset = tf.data.Dataset.from_tensor_slices(["a b c", "d e", "a f e"])
         dataset = dataset.map(tokenizer)
         dataset = dataset.apply(
@@ -204,36 +191,14 @@
             original_tokenizer.get_config()
         )
         self.assertAllEqual(
             original_tokenizer(input_data),
             cloned_tokenizer(input_data),
         )
 
-    @pytest.mark.tf_only
-    def test_saved_model(self):
-        input_data = tf.constant(["quick brOWN whale"])
-        vocab_data = ["@UNK@", "qu", "@@ick", "br", "@@OWN", "fox"]
-        tokenizer = WordPieceTokenizer(
-            vocabulary=vocab_data,
-            lowercase=False,
-            oov_token="@UNK@",
-            suffix_indicator="@@",
-            dtype="string",
-        )
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = tokenizer(inputs)
-        model = keras.Model(inputs, outputs)
-        path = os.path.join(self.get_temp_dir(), "model.keras")
-        model.save(path, save_format="keras_v3")
-        restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data),
-            restored_model(input_data),
-        )
-
     def test_no_oov_token_in_vocabulary(self):
         vocab_data = ["qu", "@@ick", "br", "@@OWN", "fox"]
         with self.assertRaises(ValueError):
             WordPieceTokenizer(
                 vocabulary=vocab_data,
             )
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/utils/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/utils/keras_utils.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/utils/keras_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/utils/keras_utils_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/utils/keras_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/utils/pipeline_model.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/utils/pipeline_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,23 @@
                 "`batch_size`. Received: "
                 f"`type(batch_size)={type(batch_size)}`."
             )
         return x
 
     inputs = pack_x_y_sample_weight(x, y, sample_weight)
     try:
+
+        def convert(x):
+            if isinstance(x, (tf.Tensor, tf.RaggedTensor)):
+                return x
+            if hasattr(x, "__array__"):
+                return ops.convert_to_numpy(x)
+            return x
+
+        inputs = tf.nest.map_structure(convert, inputs)
         ds = tf.data.Dataset.from_tensor_slices(inputs)
     except ValueError as e:
         # If our inputs are unbatched, re-raise with a more friendly error
         # message the default from tf.data. We expect this to come up with
         # some frequency, so it's important to have a good sign post here.
         if "only supported for rank >= 1" in str(e):
             raise ValueError(
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/utils/pipeline_model_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/utils/pipeline_model_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
+import numpy as np
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.backend import ops
 from keras_nlp.src.tests.test_case import TestCase
 from keras_nlp.src.utils.pipeline_model import PipelineModel
 
 
 class NoopPipeline(PipelineModel):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
@@ -85,63 +85,63 @@
     @classmethod
     def from_config(cls, config):
         return cls(**config)
 
 
 class TestNoopPipelineModel(TestCase):
     def test_fit(self):
-        x = ops.random.uniform((8, 5))
-        y = ops.random.uniform((8, 1))
-        sw = ops.random.uniform((8, 1))
+        x = np.random.uniform(size=(8, 5))
+        y = np.random.uniform(size=(8, 1))
+        sw = np.random.uniform(size=(8, 1))
         model = NoopPipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.fit(x=x, y=y, sample_weight=sw, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.fit(x=x, y=y, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_evaluate(self):
-        x = ops.random.uniform((8, 5))
-        y = ops.random.uniform((8, 1))
-        sw = ops.random.uniform((8, 1))
+        x = np.random.uniform(size=(8, 5))
+        y = np.random.uniform(size=(8, 1))
+        sw = np.random.uniform(size=(8, 1))
         model = NoopPipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.evaluate(x=x, y=y, sample_weight=sw, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.evaluate(x=x, y=y, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_predict(self):
-        x = ops.random.uniform((8, 5))
+        x = np.random.uniform(size=(8, 5))
         model = NoopPipeline()
         model.compile(loss="mse")
         model.predict(x=x, batch_size=8)
         model.predict(tf.data.Dataset.from_tensor_slices(x).batch(8))
 
     def test_on_batch(self):
-        x = ops.random.uniform((8, 5))
-        y = ops.random.uniform((8, 1))
-        sw = ops.random.uniform((8, 1))
+        x = np.random.uniform(size=(8, 5))
+        y = np.random.uniform(size=(8, 1))
+        sw = np.random.uniform(size=(8, 1))
         model = NoopPipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.train_on_batch(x=x, y=y, sample_weight=sw)
         model.test_on_batch(x=x, y=y, sample_weight=sw)
         # Without sample weight.
         model.train_on_batch(x=x, y=y)
         model.test_on_batch(x=x, y=y)
         model.predict_on_batch(x=x)
 
     def test_saved_model(self):
         model = NoopPipeline()
-        x = ops.random.uniform((8, 5))
+        x = np.random.uniform(size=(8, 5))
         model_output = model.predict(x)
         path = os.path.join(self.get_temp_dir(), "model.keras")
         model.save(path, save_format="keras_v3")
         restored_model = keras.models.load_model(
             path, custom_objects={"NoopPipeline": NoopPipeline}
         )
 
@@ -150,109 +150,109 @@
         # Check that output matches.
         restored_output = restored_model.predict(x)
         self.assertAllClose(model_output, restored_output)
 
 
 class TestFeaturePreprocessingModel(TestCase):
     def test_fit_with_preprocessing(self):
-        x = tf.strings.as_string(ops.random.uniform((100, 5)))
-        y = ops.random.uniform((100, 1))
-        sw = ops.random.uniform((100, 1))
+        x = tf.strings.as_string(np.random.uniform(size=(100, 5)))
+        y = np.random.uniform(size=(100, 1))
+        sw = np.random.uniform(size=(100, 1))
         model = FeaturePipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.fit(x=x, y=y, sample_weight=sw, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.fit(x=x, y=y, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_fit_no_preprocessing(self):
-        x = ops.random.uniform((100, 5))
-        y = ops.random.uniform((100, 1))
-        sw = ops.random.uniform((100, 1))
+        x = np.random.uniform(size=(100, 5))
+        y = np.random.uniform(size=(100, 1))
+        sw = np.random.uniform(size=(100, 1))
         model = FeaturePipeline(include_preprocessing=False)
         model.compile(loss="mse")
         # With sample weight.
         model.fit(x=x, y=y, sample_weight=sw, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.fit(x=x, y=y, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_evaluate_with_preprocessing(self):
-        x = tf.strings.as_string(ops.random.uniform((100, 5)))
-        y = ops.random.uniform((100, 1))
-        sw = ops.random.uniform((100, 1))
+        x = tf.strings.as_string(np.random.uniform(size=(100, 5)))
+        y = np.random.uniform(size=(100, 1))
+        sw = np.random.uniform(size=(100, 1))
         model = FeaturePipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.evaluate(x=x, y=y, sample_weight=sw, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.evaluate(x=x, y=y, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_evaluate_no_preprocessing(self):
-        x = ops.random.uniform((100, 5))
-        y = ops.random.uniform((100, 1))
-        sw = ops.random.uniform((100, 1))
+        x = np.random.uniform(size=(100, 5))
+        y = np.random.uniform(size=(100, 1))
+        sw = np.random.uniform(size=(100, 1))
         model = FeaturePipeline(include_preprocessing=False)
         model.compile(loss="mse")
         # With sample weight.
         model.evaluate(x=x, y=y, sample_weight=sw, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.evaluate(x=x, y=y, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_predict_with_preprocessing(self):
-        x = tf.strings.as_string(ops.random.uniform((100, 5)))
+        x = tf.strings.as_string(np.random.uniform(size=(100, 5)))
         model = FeaturePipeline()
         model.compile(loss="mse")
         model.predict(x=x, batch_size=8)
         model.predict(tf.data.Dataset.from_tensor_slices(x).batch(8))
 
     def test_predict_no_preprocessing(self):
-        x = ops.random.uniform((100, 5))
+        x = np.random.uniform(size=(100, 5))
         model = FeaturePipeline(include_preprocessing=False)
         model.compile(loss="mse")
         model.predict(x=x, batch_size=8)
         model.predict(tf.data.Dataset.from_tensor_slices(x).batch(8))
 
     def test_on_batch(self):
-        x = tf.strings.as_string(ops.random.uniform((8, 5)))
-        y = ops.random.uniform((8, 1))
-        sw = ops.random.uniform((8, 1))
+        x = tf.strings.as_string(np.random.uniform(size=(8, 5)))
+        y = np.random.uniform(size=(8, 1))
+        sw = np.random.uniform(size=(8, 1))
         model = FeaturePipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.train_on_batch(x=x, y=y, sample_weight=sw)
         model.test_on_batch(x=x, y=y, sample_weight=sw)
         # Without sample weight.
         model.train_on_batch(x=x, y=y)
         model.test_on_batch(x=x, y=y)
         model.predict_on_batch(x=x)
 
     def test_on_batch_no_preprocessing(self):
-        x = ops.random.uniform((8, 5))
-        y = ops.random.uniform((8, 1))
-        sw = ops.random.uniform((8, 1))
+        x = np.random.uniform(size=(8, 5))
+        y = np.random.uniform(size=(8, 1))
+        sw = np.random.uniform(size=(8, 1))
         model = FeaturePipeline(include_preprocessing=False)
         model.compile(loss="mse")
         # With sample weight.
         model.train_on_batch(x=x, y=y, sample_weight=sw)
         model.test_on_batch(x=x, y=y, sample_weight=sw)
         # Without sample weight.
         model.train_on_batch(x=x, y=y)
         model.test_on_batch(x=x, y=y)
 
     def test_saved_model(self):
         model = FeaturePipeline()
-        x = tf.strings.as_string(ops.random.uniform((8, 5)))
+        x = tf.strings.as_string(np.random.uniform(size=(8, 5)))
         model_output = model.predict(x)
         path = os.path.join(self.get_temp_dir(), "model.keras")
         model.save(path, save_format="keras_v3")
         restored_model = keras.models.load_model(
             path, custom_objects={"FeaturePipeline": FeaturePipeline}
         )
 
@@ -261,103 +261,103 @@
         # Check that output matches.
         restored_output = restored_model.predict(x)
         self.assertAllClose(model_output, restored_output)
 
 
 class TestLabelPreprocessingModel(TestCase):
     def test_fit_with_preprocessing(self):
-        x = ops.random.uniform((100, 5))
-        y = tf.strings.as_string(ops.random.uniform((100, 1)))
-        sw = ops.random.uniform((100, 1))
+        x = np.random.uniform(size=(100, 5))
+        y = tf.strings.as_string(np.random.uniform(size=(100, 1)))
+        sw = np.random.uniform(size=(100, 1))
         model = LabelPipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.fit(x=x, y=y, sample_weight=sw, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.fit(x=x, y=y, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_fit_no_preprocessing(self):
-        x = ops.random.uniform((100, 5))
-        y = ops.random.uniform((100, 1))
-        sw = ops.random.uniform((100, 1))
+        x = np.random.uniform(size=(100, 5))
+        y = np.random.uniform(size=(100, 1))
+        sw = np.random.uniform(size=(100, 1))
         model = LabelPipeline(include_preprocessing=False)
         model.compile(loss="mse")
         # With sample weight.
         model.fit(x=x, y=y, sample_weight=sw, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.fit(x=x, y=y, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_evaluate_with_preprocessing(self):
-        x = ops.random.uniform((100, 5))
-        y = tf.strings.as_string(ops.random.uniform((100, 1)))
-        sw = ops.random.uniform((100, 1))
+        x = np.random.uniform(size=(100, 5))
+        y = tf.strings.as_string(np.random.uniform(size=(100, 1)))
+        sw = np.random.uniform(size=(100, 1))
         model = LabelPipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.evaluate(x=x, y=y, sample_weight=sw, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.evaluate(x=x, y=y, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_evaluate_no_preprocessing(self):
-        x = ops.random.uniform((100, 5))
-        y = ops.random.uniform((100, 1))
-        sw = ops.random.uniform((100, 1))
+        x = np.random.uniform(size=(100, 5))
+        y = np.random.uniform(size=(100, 1))
+        sw = np.random.uniform(size=(100, 1))
         model = LabelPipeline(include_preprocessing=False)
         model.compile(loss="mse")
         # With sample weight.
         model.evaluate(x=x, y=y, sample_weight=sw, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.evaluate(x=x, y=y, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_predict_with_preprocessing(self):
-        x = ops.random.uniform((100, 5))
+        x = np.random.uniform(size=(100, 5))
         model = LabelPipeline()
         model.compile(loss="mse")
         model.predict(x=x, batch_size=8)
         model.predict(tf.data.Dataset.from_tensor_slices(x).batch(8))
 
     def test_on_batch(self):
-        x = ops.random.uniform((8, 5))
-        y = tf.strings.as_string(ops.random.uniform((8, 1)))
-        sw = ops.random.uniform((8, 1))
+        x = np.random.uniform(size=(8, 5))
+        y = tf.strings.as_string(np.random.uniform(size=(8, 1)))
+        sw = np.random.uniform(size=(8, 1))
         model = LabelPipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.train_on_batch(x=x, y=y, sample_weight=sw)
         model.test_on_batch(x=x, y=y, sample_weight=sw)
         # Without sample weight.
         model.train_on_batch(x=x, y=y)
         model.test_on_batch(x=x, y=y)
         model.predict_on_batch(x=x)
 
     def test_on_batch_no_preprocessing(self):
-        x = ops.random.uniform((8, 5))
-        y = ops.random.uniform((8, 1))
-        sw = ops.random.uniform((8, 1))
+        x = np.random.uniform(size=(8, 5))
+        y = np.random.uniform(size=(8, 1))
+        sw = np.random.uniform(size=(8, 1))
         model = LabelPipeline(include_preprocessing=False)
         model.compile(loss="mse")
         # With sample weight.
         model.train_on_batch(x=x, y=y, sample_weight=sw)
         model.test_on_batch(x=x, y=y, sample_weight=sw)
         # Without sample weight.
         model.train_on_batch(x=x, y=y)
         model.test_on_batch(x=x, y=y)
         model.predict_on_batch(x=x)
 
     def test_saved_model(self):
         model = LabelPipeline()
-        x = ops.random.uniform((8, 5))
+        x = np.random.uniform(size=(8, 5))
         model_output = model.predict(x)
         path = os.path.join(self.get_temp_dir(), "model.keras")
         model.save(path, save_format="keras_v3")
         restored_model = keras.models.load_model(
             path, custom_objects={"LabelPipeline": LabelPipeline}
         )
 
@@ -366,86 +366,86 @@
         # Check that output matches.
         restored_output = restored_model.predict(x)
         self.assertAllClose(model_output, restored_output)
 
 
 class TestDataPreprocessingModel(TestCase):
     def test_fit_with_preprocessing(self):
-        data = tf.strings.as_string(ops.random.uniform((100, 1)))
+        data = tf.strings.as_string(np.random.uniform(size=(100, 1)))
         model = DataPipeline()
         model.compile(loss="mse")
         model.fit(x=data, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices(data).batch(8))
 
     def test_fit_no_preprocessing(self):
-        x = ops.random.uniform((100, 1))
-        y = ops.random.uniform((100, 1))
+        x = np.random.uniform(size=(100, 1))
+        y = np.random.uniform(size=(100, 1))
         model = DataPipeline(include_preprocessing=False)
         model.compile(loss="mse")
         model.fit(x=x, y=y, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_evaluate_with_preprocessing(self):
-        data = tf.strings.as_string(ops.random.uniform((100, 1)))
+        data = tf.strings.as_string(np.random.uniform(size=(100, 1)))
         model = DataPipeline()
         model.compile(loss="mse")
         model.evaluate(x=data, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices(data).batch(8))
 
     def test_evaluate_no_preprocessing(self):
-        x = ops.random.uniform((100, 1))
-        y = ops.random.uniform((100, 1))
+        x = np.random.uniform(size=(100, 1))
+        y = np.random.uniform(size=(100, 1))
         model = DataPipeline(include_preprocessing=False)
         model.compile(loss="mse")
         model.evaluate(x=x, y=y, batch_size=8)
         model.evaluate(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_predict_with_preprocessing(self):
-        x = tf.strings.as_string(ops.random.uniform((100, 1)))
+        x = tf.strings.as_string(np.random.uniform(size=(100, 1)))
         model = DataPipeline()
         model.compile(loss="mse")
         model.predict(x=x, batch_size=8)
         model.predict(tf.data.Dataset.from_tensor_slices(x).batch(8))
 
     def test_predict_no_preprocessing(self):
-        x = ops.random.uniform((100, 1))
+        x = np.random.uniform(size=(100, 1))
         model = DataPipeline(include_preprocessing=False)
         model.compile(loss="mse")
         model.predict(x=x, batch_size=8)
         model.predict(tf.data.Dataset.from_tensor_slices(x).batch(8))
 
     def test_on_batch(self):
-        data = tf.strings.as_string(ops.random.uniform((8, 1)))
+        data = tf.strings.as_string(np.random.uniform(size=(8, 1)))
         model = DataPipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.train_on_batch(x=data)
         model.test_on_batch(x=data)
         # Without sample weight.
         model.train_on_batch(x=data)
         model.test_on_batch(x=data)
         model.predict_on_batch(x=data)
 
     def test_on_batch_no_preprocessing(self):
-        x = ops.random.uniform((8, 1))
-        y = ops.random.uniform((8, 1))
-        sw = ops.random.uniform((8, 1))
+        x = np.random.uniform(size=(8, 1))
+        y = np.random.uniform(size=(8, 1))
+        sw = np.random.uniform(size=(8, 1))
         model = DataPipeline(include_preprocessing=False)
         model.compile(loss="mse")
         # With sample weight.
         model.train_on_batch(x=x, y=y, sample_weight=sw)
         model.test_on_batch(x=x, y=y, sample_weight=sw)
         # Without sample weight.
         model.train_on_batch(x=x, y=y)
         model.test_on_batch(x=x, y=y)
         model.predict_on_batch(x=x)
 
     def test_saved_model(self):
         model = DataPipeline()
-        data = tf.strings.as_string(ops.random.uniform((8, 1)))
+        data = tf.strings.as_string(np.random.uniform(size=(8, 1)))
         model_output = model.predict(data)
         path = os.path.join(self.get_temp_dir(), "model.keras")
         model.save(path, save_format="keras_v3")
         restored_model = keras.models.load_model(
             path, custom_objects={"DataPipeline": DataPipeline}
         )
 
@@ -454,43 +454,43 @@
         # Check that output matches.
         restored_output = restored_model.predict(data)
         self.assertAllClose(model_output, restored_output)
 
 
 class TestFunctional(TestCase):
     def test_fit(self):
-        x = tf.strings.as_string(ops.random.uniform((100, 5)))
-        y = ops.random.uniform((100, 1))
-        sw = ops.random.uniform((100, 1))
+        x = tf.strings.as_string(np.random.uniform(size=(100, 5)))
+        y = np.random.uniform(size=(100, 1))
+        sw = np.random.uniform(size=(100, 1))
 
         model = FunctionalPipeline()
         model.compile(loss="mse")
         # With sample weight.
         model.fit(x=x, y=y, sample_weight=sw, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.fit(x=x, y=y, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_fit_no_preprocessing(self):
-        x = ops.random.uniform((100, 5))
-        y = ops.random.uniform((100, 1))
-        sw = ops.random.uniform((100, 1))
+        x = np.random.uniform(size=(100, 5))
+        y = np.random.uniform(size=(100, 1))
+        sw = np.random.uniform(size=(100, 1))
         model = FunctionalPipeline(include_preprocessing=False)
         model.compile(loss="mse")
         # With sample weight.
         model.fit(x=x, y=y, sample_weight=sw, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y, sw)).batch(8))
         # Without sample weight.
         model.fit(x=x, y=y, batch_size=8)
         model.fit(tf.data.Dataset.from_tensor_slices((x, y)).batch(8))
 
     def test_saved_model(self):
         model = FunctionalPipeline()
-        x = tf.strings.as_string(ops.random.uniform((8, 5)))
+        x = tf.strings.as_string(np.random.uniform(size=(8, 5)))
         model_output = model.predict(x)
         path = os.path.join(self.get_temp_dir(), "model.keras")
         model.save(path, save_format="keras_v3")
         restored_model = keras.models.load_model(
             path, custom_objects={"FunctionalPipeline": FunctionalPipeline}
         )
 
@@ -499,43 +499,43 @@
         # Check that output matches.
         restored_output = restored_model.predict(x)
         self.assertAllClose(model_output, restored_output)
 
 
 class TestFitArguments(TestCase):
     def test_validation_data(self):
-        x = tf.strings.as_string(ops.random.uniform((80, 5)))
-        y = ops.random.uniform((80, 1))
-        val_x = tf.strings.as_string(ops.random.uniform((20, 5)))
-        val_y = ops.random.uniform((20, 1))
+        x = tf.strings.as_string(np.random.uniform(size=(80, 5)))
+        y = np.random.uniform(size=(80, 1))
+        val_x = tf.strings.as_string(np.random.uniform(size=(20, 5)))
+        val_y = np.random.uniform(size=(20, 1))
 
         model = FeaturePipeline()
         model.compile(loss="mse")
 
         model.fit(x=x, y=y, validation_data=(val_x, val_y), batch_size=8)
         model.fit(
             x=tf.data.Dataset.from_tensor_slices((x, y)).batch(8),
             validation_data=tf.data.Dataset.from_tensor_slices(
                 (val_x, val_y)
             ).batch(8),
         )
 
     def test_validation_split(self):
-        x = tf.strings.as_string(ops.random.uniform((100, 5)))
-        y = ops.random.uniform((100, 1))
+        x = tf.strings.as_string(np.random.uniform(size=(100, 5)))
+        y = np.random.uniform(size=(100, 1))
 
         model = FeaturePipeline()
         model.compile(loss="mse")
 
         model.fit(x=x, y=y, validation_split=0.2, batch_size=8)
 
     def test_error_dataset_and_invalid_arguments(self):
-        x = tf.strings.as_string(ops.random.uniform((100, 5)))
-        y = ops.random.uniform((100, 1))
-        sw = ops.random.uniform((100, 1))
+        x = tf.strings.as_string(np.random.uniform(size=(100, 5)))
+        y = np.random.uniform(size=(100, 1))
+        sw = np.random.uniform(size=(100, 1))
         ds = tf.data.Dataset.from_tensor_slices((x, y))
 
         model = FeaturePipeline()
         model.compile(loss="mse")
         with self.assertRaises(ValueError):
             model.fit(ds, validation_split=0.2)
         with self.assertRaises(ValueError):
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/utils/python_utils.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/utils/python_utils_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/utils/python_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/utils/tensor_utils.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/utils/tensor_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     tf_text = None
 
 
 def _decode_strings_to_utf8(inputs):
     """Recursively decodes to list of strings with 'utf-8' encoding."""
     if isinstance(inputs, bytes):
         # Handles the case when the input is a scalar string.
-        return inputs.decode("utf-8")
+        return inputs.decode("utf-8", errors="ignore")
     else:
         # Recursively iterate when input is a list.
         return [_decode_strings_to_utf8(x) for x in inputs]
 
 
 def tensor_to_list(inputs):
     """Converts a tensor to nested lists.
@@ -79,32 +79,35 @@
 
     Returns:
         An `(inputs, unbatched, rectangular)` tuple, where `inputs` is a
         2-D `tf.RaggedTensor`, `unbatched` is `True` if the inputs were
         origianlly rank 1, and `rectangular` is `True` if the inputs rows are
         all of equal lengths.
     """
-    rectangular = True
     # `tf.keras.layers.Layer` does a weird conversion in __call__, where a list
     # of lists of ints will become a list of list of scalar tensors. We could
     # clean this up if we no longer need to care about that case.
     if isinstance(inputs, (list, tuple)):
         if isinstance(inputs[0], (list, tuple)):
             rectangular = len(set([len(row) for row in inputs])) == 1
             rows = [
                 tf.convert_to_tensor(row, dtype_hint="int32") for row in inputs
             ]
             inputs = tf.ragged.stack(rows).with_row_splits_dtype("int64")
         else:
             inputs = tf.convert_to_tensor(inputs)
+            rectangular = True
+    elif isinstance(inputs, tf.Tensor):
+        rectangular = True
     elif isinstance(inputs, tf.RaggedTensor):
         rectangular = False
     elif hasattr(inputs, "__array__"):
-        inputs = tf.convert_to_tensor(inputs)
-    elif not isinstance(inputs, tf.RaggedTensor):
+        inputs = tf.convert_to_tensor(ops.convert_to_numpy(inputs))
+        rectangular = True
+    else:
         raise ValueError(
             f"Unknown tensor type. Tensor input can be passed as "
             "tensors, numpy arrays, or python lists. Received: "
             f"`type(inputs)={type(inputs)}`"
         )
     if inputs.shape.rank < 1 or inputs.shape.rank > 2:
         raise ValueError(
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/src/utils/tensor_utils_test.py` & `keras-nlp-0.6.1.dev0/keras_nlp/src/utils/tensor_utils_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,19 @@
         self.assertAllEqual(detokenize_output, [["▀▁▂▃", "samurai"]])
 
     def test_scalar_string(self):
         input_data = tf.constant("▀▁▂▃")
         detokenize_output = tensor_to_list(input_data)
         self.assertEqual(detokenize_output, "▀▁▂▃")
 
+    def test_string_with_utf8_error(self):
+        input_data = tf.constant([b"hello\xf2\xf1\x91\xe5"])
+        detokenize_output = tensor_to_list(input_data)
+        self.assertEqual(detokenize_output, ["hello"])
+
 
 class ConvertToRaggedBatch(TestCase):
     def test_convert_1d_python(self):
         inputs = [1, 2]
         outputs, unbatched, rectangular = convert_to_ragged_batch(inputs)
         self.assertIsInstance(outputs, tf.RaggedTensor)
         self.assertAllEqual(outputs, [[1, 2]])
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp/tokenizers/__init__.py` & `keras-nlp-0.6.1.dev0/keras_nlp/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp.egg-info/PKG-INFO` & `keras-nlp-0.6.1.dev0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.6.0.dev0
+Version: 0.6.1.dev0
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -25,21 +25,24 @@
 
 # KerasNLP: Modular NLP Workflows for Keras
 [![](https://github.com/keras-team/keras-nlp/workflows/Tests/badge.svg?branch=master)](https://github.com/keras-team/keras-nlp/actions?query=workflow%3ATests+branch%3Amaster)
 ![Python](https://img.shields.io/badge/python-v3.8.0+-success.svg)
 ![Tensorflow](https://img.shields.io/badge/tensorflow-v2.5.0+-success.svg)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/keras-team/keras-nlp/issues)
 
-
-KerasNLP is a natural language processing library that supports users through
-their entire development cycle. Our workflows are built from modular components 
-that have state-of-the-art preset weights and architectures when used 
-out-of-the-box and are easily customizable when more control is needed. We 
-emphasize in-graph computation for all workflows so that developers can expect 
-easy productionization using the TensorFlow ecosystem.
+KerasNLP is a natural language processing library that works natively 
+with TensorFlow, JAX, or PyTorch. Built on [Keras Core](https://keras.io/keras_core/announcement/),
+these models, layers, metrics, callbacks, etc., can be trained and serialized
+in any framework and re-used in another without costly migrations. See "Using 
+KerasNLP with Keras Core" below for more details on multi-framework KerasNLP.
+
+KerasNLP supports users through their entire development cycle. Our workflows 
+are built from modular components that have state-of-the-art preset weights and 
+architectures when used out-of-the-box and are easily customizable when more 
+control is needed.
 
 This library is an extension of the core Keras API; all high-level modules are 
 [`Layers`](https://keras.io/api/layers/) or 
 [`Models`](https://keras.io/api/models/) that receive that same level of polish 
 as core Keras. If you are familiar with Keras, congratulations! You already 
 understand most of KerasNLP.
 
@@ -77,14 +80,42 @@
 
 To install the latest unreleased changes to the library, we recommend using
 pip to install directly from the master branch on github:
 
 ```
 pip install git+https://github.com/keras-team/keras-nlp.git --upgrade
 ```
+## Using KerasNLP with Keras Core
+
+As of version `0.6.0`, KerasNLP supports multiple backends with Keras Core out 
+of the box. There are two ways to configure KerasNLP to run with multi-backend 
+support:
+
+1. Via the `KERAS_BACKEND` environment variable. If set, then KerasNLP will be 
+using Keras Core with the backend specified (e.g., `KERAS_BACKEND=jax`).
+2. Via the `.keras/keras.json` and `.keras/keras_nlp.json` config files (which 
+are automatically created the first time you import KerasNLP):
+   - Set your backend of choice in `.keras/keras.json`; e.g., `"backend": "jax"`. 
+   - Set `"multi_backend": True` in `.keras/keras_nlp.json`.
+
+Once that configuration step is done, you can just import KerasNLP and start 
+using it on top of your backend of choice:
+
+```python
+import keras_nlp
+
+gpt2_lm = keras_nlp.models.GPT2CausalLM.from_preset("gpt2_base_en")
+gpt2_lm.generate("My trip to Yosemite was", max_length=200)
+```
+
+Until Keras Core is officially released as Keras 3.0, KerasNLP will use 
+`tf.keras` as the default backend. To restore this default behavior, simply 
+`unset KERAS_BACKEND` and ensure that  `"multi_backend": False` or is unset in 
+`.keras/keras_nlp.json`. You will need to restart the Python runtime for changes 
+to take effect.
 
 ## Quickstart
 
 Fine-tune BERT on a small sentiment analysis task using the 
 [`keras_nlp.models`](https://keras.io/api/keras_nlp/models/) API:
 
 ```python
```

### Comparing `keras-nlp-0.6.0.dev0/keras_nlp.egg-info/SOURCES.txt` & `keras-nlp-0.6.1.dev0/keras_nlp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -173,16 +173,18 @@
 keras_nlp/src/models/gpt2/gpt2_presets_test.py
 keras_nlp/src/models/gpt2/gpt2_tokenizer.py
 keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py
 keras_nlp/src/models/gpt_neo_x/__init__.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_attention.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone_test.py
+keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor_test.py
+keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_test.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_decoder.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor_test.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer_test.py
 keras_nlp/src/models/gpt_neo_x/rotary_embedding.py
 keras_nlp/src/models/opt/__init__.py
```

### Comparing `keras-nlp-0.6.0.dev0/setup.cfg` & `keras-nlp-0.6.1.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.6.0.dev0/setup.py` & `keras-nlp-0.6.1.dev0/setup.py`

 * *Files identical despite different names*


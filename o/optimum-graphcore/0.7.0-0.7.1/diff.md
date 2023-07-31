# Comparing `tmp/optimum-graphcore-0.7.0.tar.gz` & `tmp/optimum-graphcore-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-graphcore-0.7.0.tar", last modified: Thu Jul 13 12:42:16 2023, max compression
+gzip compressed data, was "optimum-graphcore-0.7.1.tar", last modified: Mon Jul 31 09:34:03 2023, max compression
```

## Comparing `optimum-graphcore-0.7.0.tar` & `optimum-graphcore-0.7.1.tar`

### file list

```diff
@@ -1,126 +1,147 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/MANIFEST.in
--rw-rw-r--   0 michael   (1000) michael   (1000)     9947 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     8905 2023-05-25 15:19:02.000000 optimum-graphcore-0.7.0/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.409396 optimum-graphcore-0.7.0/optimum/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2776 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/data/
--rw-rw-r--   0 michael   (1000) michael   (1000)      885 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/optimum/graphcore/data/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5974 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/data/data_collator.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/
--rw-rw-r--   0 michael   (1000) michael   (1000)      808 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/
--rw-rw-r--   0 michael   (1000) michael   (1000)      815 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/
--rw-rw-r--   0 michael   (1000) michael   (1000)      915 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5563 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      831 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      852 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      852 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    19051 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2335 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/generation/
--rw-rw-r--   0 michael   (1000) michael   (1000)      740 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/generation/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    17488 2023-07-13 12:41:16.000000 optimum-graphcore-0.7.0/optimum/graphcore/generation/attention_mixin.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10938 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/generation/logits_process.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    20324 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/generation/on_device_generation.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    94451 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/generation/utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    38450 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/ipu_configuration.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5749 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/optimum/graphcore/modelcard.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    33652 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/modeling_utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/
--rw-rw-r--   0 michael   (1000) michael   (1000)      954 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/bart/
--rw-rw-r--   0 michael   (1000) michael   (1000)      940 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/bart/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    50037 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/bart/modeling_bart.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/bert/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1089 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/bert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6853 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/bert/bert_fused_attention.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    22296 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/bert/modeling_bert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/
--rw-rw-r--   0 michael   (1000) michael   (1000)      906 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2801 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/modeling_convnext.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1711 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/optimized_convnextlayer.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/deberta/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1035 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/deberta/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    22415 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/deberta/modeling_deberta.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/distilbert/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1092 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/distilbert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    15150 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/distilbert/modeling_distilbert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/
--rw-rw-r--   0 michael   (1000) michael   (1000)      981 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    15345 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/modeling_gpt2.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2342 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/optimized_gpt2_attn.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1915 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10189 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_attention.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3297 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_convolution.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2892 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_ffn.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    35135 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/modeling_groupbert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/
--rw-rw-r--   0 michael   (1000) michael   (1000)      905 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6676 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/ipu_layer_drop.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8092 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/modeling_hubert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/lxmert/
--rw-rw-r--   0 michael   (1000) michael   (1000)      900 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/lxmert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6262 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/lxmert/modeling_lxmert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/mt5/
--rw-rw-r--   0 michael   (1000) michael   (1000)      898 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/mt5/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    27287 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/mt5/modeling_mt5.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/roberta/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1074 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/roberta/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    14589 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/roberta/modeling_roberta.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/t5/
--rw-rw-r--   0 michael   (1000) michael   (1000)      921 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/t5/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      777 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/t5/configuration_t5.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    25981 2023-07-13 12:41:16.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/t5/modeling_t5.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/vit/
--rw-rw-r--   0 michael   (1000) michael   (1000)      896 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/vit/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2217 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/vit/modeling_vit.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/
--rw-rw-r--   0 michael   (1000) michael   (1000)      923 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4484 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     7591 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    24472 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1029 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2256 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/feature_extraction_whisper.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    28245 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/modeling_whisper.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1226 2023-05-25 15:19:02.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/processing_whisper.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/
--rw-rw-r--   0 michael   (1000) michael   (1000)    20752 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5609 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/automatic_speech_recognition.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1873 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/fill_mask.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3696 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/text2text_generation.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1908 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/token_classification.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4471 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/zero_shot_classification.py
--rw-rw-r--   0 michael   (1000) michael   (1000)   107720 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/trainer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      987 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/optimum/graphcore/trainer_pt_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    17320 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/trainer_seq2seq.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2331 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/trainer_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    46931 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/training_args.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4528 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/training_args_seq2seq.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1128 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/optimum/graphcore/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      697 2023-07-13 12:41:16.000000 optimum-graphcore-0.7.0/optimum/graphcore/version.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     9947 2023-07-13 12:42:16.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     4352 2023-07-13 12:42:16.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-07-13 12:42:16.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-05 12:57:36.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      285 2023-07-13 12:42:16.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-07-13 12:42:16.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)     1098 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      112 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     3021 2023-07-13 12:41:40.000000 optimum-graphcore-0.7.0/setup.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)    23442 2023-07-13 12:41:16.000000 optimum-graphcore-0.7.0/tests/test_examples.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3395 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_examples_match_transformers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    25297 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_ipu_configuration.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     1808 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_modeling_common.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6691 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_modeling_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    13055 2023-07-13 12:41:16.000000 optimum-graphcore-0.7.0/tests/test_pipelined_models.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    61608 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_trainer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5653 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_trainer_seq2seq.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.156248 optimum-graphcore-0.7.1/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.1/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.1/MANIFEST.in
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9947 2023-07-31 09:34:03.156248 optimum-graphcore-0.7.1/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8905 2023-05-25 15:19:02.000000 optimum-graphcore-0.7.1/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.144248 optimum-graphcore-0.7.1/optimum/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.148248 optimum-graphcore-0.7.1/optimum/graphcore/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2876 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.148248 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.148248 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/group_quantize_decompress/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1322 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/group_quantize_decompress/common.hpp
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4707 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/group_quantize_decompress/group_quantize_decompress.cpp
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1672 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/group_quantize_decompress/group_quantize_decompress.hpp
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4489 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/group_quantize_decompress/group_quantize_decompress_codelet_v1.cpp
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5821 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/group_quantize_decompress/group_quantize_decompressx.cpp
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1052 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/group_quantize_decompress/group_quantize_decompressx.hpp
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.148248 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/sdk_version_hash/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      645 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/sdk_version_hash/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      910 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/sdk_version_hash/sdk_version_hash.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1628 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/sdk_version_hash/sdk_version_hash_lib.cpp
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3879 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/custom_ops/utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.148248 optimum-graphcore-0.7.1/optimum/graphcore/data/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      885 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.1/optimum/graphcore/data/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5974 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/data/data_collator.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.148248 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      808 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.148248 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      815 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.148248 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      915 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5563 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      831 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      852 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      852 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    19051 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2335 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/generation/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      740 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/generation/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    18367 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/generation/attention_mixin.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10938 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/generation/logits_process.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    20324 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/generation/on_device_generation.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    94619 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/generation/utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    39696 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/ipu_configuration.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5749 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.1/optimum/graphcore/modelcard.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    34502 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/modeling_utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      954 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/bart/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      940 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/bart/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    50027 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/bart/modeling_bart.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/bert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1113 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/bert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6853 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/bert/bert_fused_attention.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    24678 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/bert/modeling_bert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/convnext/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      906 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/convnext/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2801 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/convnext/modeling_convnext.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1711 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/convnext/optimized_convnextlayer.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/deberta/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1035 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/deberta/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22415 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/deberta/modeling_deberta.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/distilbert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1092 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/distilbert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15150 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/distilbert/modeling_distilbert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/gpt2/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      981 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/gpt2/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15345 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/gpt2/modeling_gpt2.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2342 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/gpt2/optimized_gpt2_attn.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1915 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10189 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/groupbert_attention.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3297 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/groupbert_convolution.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2892 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/groupbert_ffn.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    35135 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/modeling_groupbert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/hubert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      905 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/hubert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6676 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/hubert/ipu_layer_drop.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8092 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/hubert/modeling_hubert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/lxmert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      900 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/lxmert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6262 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/lxmert/modeling_lxmert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/mpnet/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      866 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/mpnet/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7972 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/mpnet/modeling_mpnet.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/mt5/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      898 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/mt5/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    27287 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/mt5/modeling_mt5.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/roberta/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1074 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/roberta/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14589 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/roberta/modeling_roberta.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/t5/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      921 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/t5/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      777 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/t5/configuration_t5.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    38492 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/t5/modeling_t5.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/vit/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      896 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/vit/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2217 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/vit/modeling_vit.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/wav2vec2/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      923 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/wav2vec2/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4484 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7591 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)    24472 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/models/whisper/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1029 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/whisper/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2256 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/whisper/feature_extraction_whisper.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    33020 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/whisper/modeling_whisper.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1226 2023-05-25 15:19:02.000000 optimum-graphcore-0.7.1/optimum/graphcore/models/whisper/processing_whisper.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.152248 optimum-graphcore-0.7.1/optimum/graphcore/pipelines/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    20812 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/pipelines/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5609 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/pipelines/automatic_speech_recognition.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1873 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/pipelines/fill_mask.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3696 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/pipelines/text2text_generation.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1908 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/pipelines/token_classification.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4471 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/pipelines/zero_shot_classification.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.156248 optimum-graphcore-0.7.1/optimum/graphcore/quantization/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      888 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/quantization/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8523 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/quantization/group_quantize.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)   110697 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/trainer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      987 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.1/optimum/graphcore/trainer_pt_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    17416 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/trainer_seq2seq.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2331 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/trainer_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    46931 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/training_args.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4528 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/optimum/graphcore/training_args_seq2seq.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.156248 optimum-graphcore-0.7.1/optimum/graphcore/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1128 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.1/optimum/graphcore/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      697 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/optimum/graphcore/version.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.156248 optimum-graphcore-0.7.1/optimum_graphcore.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9947 2023-07-31 09:34:03.000000 optimum-graphcore-0.7.1/optimum_graphcore.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5339 2023-07-31 09:34:03.000000 optimum-graphcore-0.7.1/optimum_graphcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-07-31 09:34:03.000000 optimum-graphcore-0.7.1/optimum_graphcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-05 12:57:36.000000 optimum-graphcore-0.7.1/optimum_graphcore.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      303 2023-07-31 09:34:03.000000 optimum-graphcore-0.7.1/optimum_graphcore.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-07-31 09:34:03.000000 optimum-graphcore-0.7.1/optimum_graphcore.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1098 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      112 2023-07-31 09:34:03.156248 optimum-graphcore-0.7.1/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3089 2023-07-31 09:33:27.000000 optimum-graphcore-0.7.1/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 09:34:03.156248 optimum-graphcore-0.7.1/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1044 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/tests/test_custom_ops.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    25535 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/tests/test_examples.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3395 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/tests/test_examples_match_transformers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    25297 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/tests/test_ipu_configuration.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)     1808 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/tests/test_modeling_common.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6691 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/tests/test_modeling_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14326 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/tests/test_pipelined_models.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    61608 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.1/tests/test_trainer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5649 2023-07-31 09:33:20.000000 optimum-graphcore-0.7.1/tests/test_trainer_seq2seq.py
```

### Comparing `optimum-graphcore-0.7.0/LICENSE` & `optimum-graphcore-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/MANIFEST.in` & `optimum-graphcore-0.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/PKG-INFO` & `optimum-graphcore-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-graphcore
-Version: 0.7.0
+Version: 0.7.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://huggingface.co/hardware
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,training,ipu
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `optimum-graphcore-0.7.0/README.md` & `optimum-graphcore-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #  limitations under the License.
 
 import poptorch
 
 from .ipu_configuration import IPUConfig
 from .models.bart import PipelinedBartForConditionalGeneration, PipelinedBartForSequenceClassification
 from .models.bert import (
+    PipelinedBertModel,
     PipelinedBertForMaskedLM,
     PipelinedBertForMultipleChoice,
     PipelinedBertForPreTraining,
     PipelinedBertForQuestionAnswering,
     PipelinedBertForSequenceClassification,
     PipelinedBertForTokenClassification,
 )
@@ -38,14 +39,15 @@
     PipelinedDistilBertForTokenClassification,
 )
 from .models.gpt2 import (
     PipelinedGPT2ForSequenceClassification,
     PipelinedGPT2ForTokenClassification,
     PipelinedGPT2LMHeadModel,
 )
+
 from .models.hubert import PipelinedHubertForSequenceClassification
 from .models.lxmert import PipelinedLxmertForQuestionAnswering
 from .models.mt5 import PipelinedMT5ForConditionalGeneration
 from .models.roberta import (
     PipelinedRobertaForMaskedLM,
     PipelinedRobertaForMultipleChoice,
     PipelinedRobertaForQuestionAnswering,
@@ -54,14 +56,17 @@
 )
 from .models.t5 import (
     PipelinedT5ForConditionalGeneration,
     PipelinedT5EncoderModel,
 )
 from .models.vit import PipelinedViTForImageClassification
 from .models.wav2vec2 import PipelinedWav2Vec2ForPreTraining
+
+from .models.mpnet import PipelinedMPNetModel, PipelinedMPNetForMaskedLM
+
 from .pipelines import IPUFillMaskPipeline, IPUTokenClassificationPipeline, pipeline
 from .trainer import IPUTrainer, IPUTrainerState
 from .trainer_seq2seq import IPUSeq2SeqTrainer
 from .training_args import IPUTrainingArguments
 from .training_args_seq2seq import IPUSeq2SeqTrainingArguments
 from .version import __version__
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/data/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/data/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/data/data_collator.py` & `optimum-graphcore-0.7.1/optimum/graphcore/data/data_collator.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py` & `optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py` & `optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py` & `optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py` & `optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py` & `optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py` & `optimum-graphcore-0.7.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/generation/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/generation/attention_mixin.py` & `optimum-graphcore-0.7.1/optimum/graphcore/generation/attention_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,16 @@
     def from_model(
         cls,
         attention_layer: torch.nn.Module,
         use_cache: bool = False,
         batch_size: int = 1,
         max_length: int = 128,
         num_beams: int = 1,
+        num_heads: Optional[int] = None,
+        head_dim: Optional[int] = None,
         dtype: torch.dtype = torch.float16,
         batch_serialization_factor: int = 1,
         sequence_serialization_factor: int = 1,
         use_cross_cache: bool = False,
         encoder_max_length: int = 128,
     ):
         """
@@ -116,27 +118,43 @@
 
         If `batch_serialization_factor > 1` or `sequence_serialization_factor > 1`, attention will be serialized
         along the batch or sequence dimension respectively.
         """
         clone = copy.deepcopy(attention_layer)
         clone.__class__ = cls
 
+        def infer_attribute_from_layer(attr: str):
+            err_msg = (
+                f"Attempting to replace attention class `{attention_layer.__class__.__name__}` with `{cls.__name__}`."
+                f" However unable to infer `{{0}}` from `{attention_layer.__class__.__name__}`."
+                " Provide the `{0}` argument to `IPUAttentionMixin.from_model`."
+            )
+            try:
+                value = getattr(clone, attr)
+                return value
+            except AttributeError as e:
+                raise AttributeError(err_msg.format(attr)) from e
+
+        if use_cache or use_cross_cache:
+            num_heads = infer_attribute_from_layer("num_heads") if num_heads is None else num_heads
+            head_dim = infer_attribute_from_layer("head_dim") if head_dim is None else head_dim
+
         if use_cache:
             clone._create_kv_cache(
-                (batch_size * num_beams, clone.num_heads, max_length, clone.head_dim),
+                (batch_size * num_beams, num_heads, max_length, head_dim),
                 dtype=dtype,
                 num_beams=num_beams,
             )
 
         if use_cross_cache:
             assert_poptorch_supports_cond(
                 context="Cross-attention KV caching has been enabled with `use_cross_cache=True`."
             )
             clone._create_cross_kv_cache(
-                (batch_size * num_beams, clone.num_heads, encoder_max_length, clone.head_dim),
+                (batch_size * num_beams, num_heads, encoder_max_length, head_dim),
                 dtype=dtype,
                 num_beams=num_beams,
             )
 
         if batch_serialization_factor < 1 or sequence_serialization_factor < 1:
             raise ValueError(
                 "`batch_serialization_factor` and `sequence_serialization_factor` must be > 0 if provided."
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/generation/logits_process.py` & `optimum-graphcore-0.7.1/optimum/graphcore/generation/logits_process.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/generation/on_device_generation.py` & `optimum-graphcore-0.7.1/optimum/graphcore/generation/on_device_generation.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/generation/utils.py` & `optimum-graphcore-0.7.1/optimum/graphcore/generation/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,16 @@
         elif self.encoder_output_buffer_enabled:
             encoder_last_hidden_state = kwargs.pop("encoder_outputs")["last_hidden_state"]
             attention_mask = kwargs.pop("attention_mask", None)
             if generation_step == 0:
                 self.poptorch_decoder.encoder_last_hidden_state.copy_(encoder_last_hidden_state)
                 if attention_mask is not None:
                     self.poptorch_decoder.encoder_attention_mask.copy_(attention_mask.half())
+                if self.poptorch_decoder.isCompiled() and not self.poptorch_decoder.isAttachedToDevice():
+                    self.poptorch_decoder.attachToDevice()
                 self.poptorch_decoder.copyNamedBuffersToDevice()
 
         # This will trigger a compile first time it's ran
         with graph_profile_dir_append("/decoder" if self.config.is_encoder_decoder else ""):
             return self.poptorch_decoder(*args, t=t, **kwargs)
 
     def _prepare_encoder_decoder_kwargs_for_generation(
@@ -1659,15 +1661,15 @@
         self, stopping_criteria: StoppingCriteriaList, on_device_generation_steps: int
     ):
         adapted_stopping_criteria = []
         for stopping_criterion in stopping_criteria:
             if hasattr(stopping_criterion, "max_length"):
                 max_length = stopping_criterion.max_length
                 new_max_length = max_length - on_device_generation_steps
-                logger.info(
+                logger.debug(
                     f"Temporarily adapting `max_length` from {max_length} to {new_max_length} for on device generation."
                 )
                 stopping_criterion = copy.deepcopy(stopping_criterion)
                 stopping_criterion.max_length = new_max_length
             adapted_stopping_criteria.append(stopping_criterion)
         return StoppingCriteriaList(adapted_stopping_criteria)
 
@@ -1735,15 +1737,15 @@
         batch_size, context_length = input_ids.shape
         vocab_size = self.get_output_embeddings().out_features
 
         if context_length > 1:
             raise ValueError("Context length (input_ids.shape[-1]) > 1 is not supported yet.")
 
         if (max_length - context_length) % self.on_device_generation_steps != 0:
-            logger.info(
+            logger.debug(
                 "`max_length - context_length` does not evenly divide `on_device_generation_steps` "
                 f"({max_length - context_length} vs {self.on_device_generation_steps}). Generation will be done "
                 f"{self.on_device_generation_steps} tokens at a time and stop short of `max_length` so as not to exceed it."
             )
 
         decoder_ipu_config = getattr(self, "decoder_ipu_config", self.ipu_config)
         if decoder_ipu_config.inference_device_iterations not in (1, self.on_device_generation_steps):
@@ -1837,15 +1839,15 @@
         batch_beam_size, context_length = input_ids.shape
         vocab_size = self.get_output_embeddings().out_features
 
         if context_length > 1:
             raise ValueError("Context length (input_ids.shape[-1]) > 1 is not supported yet.")
 
         if (max_length - context_length) % self.on_device_generation_steps != 0:
-            logger.info(
+            logger.debug(
                 "`max_length - context_length` does not evenly divide `on_device_generation_steps` "
                 f"({max_length - context_length} vs {self.on_device_generation_steps}). Generation will be done "
                 f"{self.on_device_generation_steps} tokens at a time and stop short of `max_length` so as not to exceed it."
             )
 
         decoder_ipu_config = getattr(self, "decoder_ipu_config", self.ipu_config)
         if decoder_ipu_config.inference_device_iterations not in (1, self.on_device_generation_steps):
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/ipu_configuration.py` & `optimum-graphcore-0.7.1/optimum/graphcore/ipu_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,18 @@
         inference_layers_per_ipu (`List[int]`):
             Same as `layers_per_ipu` for inference only.
         ipus_per_replica (`int`, *optional*, defaults to `len(layers_per_ipu)`):
             Specifies the number of IPUs to use during training. This must be consistent with
             the number of IPUs used in `layers_per_ipu`.
         inference_ipus_per_replica (`int`, *optional*, defaults to `len(inference_layers_per_ipu) if ipus_per_replica==len(layers_per_ipu) else ipus_per_replica):
             Same as `ipus_per_replica` but for inference only.
+        parallelize_kwargs (`Dict[str, Any]`, *optional*, defaults to None):
+            Dictionary holding kwargs used for training model calls to `parallelize`.
+        inference_parallelize_kwargs (`Dict[str, Any]`, *optional*, defaults to None):
+            Dictionary holding kwargs used for inference model calls to `parallelize`.
 
         > Parameters for memory management
 
         optimizer_state_offchip (`bool`, *optional*, defaults to `True`):
             If `True`, uses the off-chip memory to store the optimizer state. If `False`, uses the on-chip memory.
         replicated_tensor_sharding (`bool`, *optional*, defaults to `False`):
             Shards the optimizer between replicas with zero-redundancy.
@@ -148,14 +152,18 @@
         serialized_projection_splits_per_ipu (`List[int]`, *optional*, defaults to None):
             Analogous to `serialized_embedding_splits_per_ipu`.
             Note: only one of `projection_serialization_factor` or `serialized_projection_splits_per_ipu` should be set.
         inference_serialized_projection_splits_per_ipu (`List[int]`, *optional*, defaults to None):
             Same as `serialized_projection_splits_per_ipu` but for inference only.
         recompute_checkpoint_every_layer (`bool`, *optional*, defaults to `False`):
             If `True`, uses gradient checkpointing at the end of every layer. It can help to reduce the memory impact.
+        explicit_ir_inference (`bool`, *optional*, defaults to `False`):
+            If `True`, uses experimental explicit-IR feature of PopART for inference models. This feature is only supported
+            for inference models. For some cases explicit-IR can provide a better memory liveness schedule, reducing the peak
+            memory during runtime.
 
         > Parameters related to host/device synchronization
 
         device_iterations (`int`, *optional*, defaults to 1):
             Number of iterations the device should run over the data before returning to the user during training. This
             is equivalent to running the IPU in a loop over the specified number of iterations, with a new batch of
             data each time. However, increasing the number of device iterations is more efficient because the loop runs on the IPU
@@ -199,14 +207,15 @@
     _layers_per_ipu = ManagedAttribute("layers_per_ipu")
     _ipus_per_replica = ManagedAttribute("ipus_per_replica")
     _matmul_proportion = ManagedAttribute("matmul_proportion")
     _embedding_serialization_factor = ManagedAttribute("embedding_serialization_factor")
     _serialized_embedding_splits_per_ipu = ManagedAttribute("serialized_embedding_splits_per_ipu")
     _projection_serialization_factor = ManagedAttribute("projection_serialization_factor")
     _serialized_projection_splits_per_ipu = ManagedAttribute("serialized_projection_splits_per_ipu")
+    _parallelize_kwargs = ManagedAttribute("parallelize_kwargs")
 
     # Create a mapping of attributes to their list of validation functions
     attribute_validators = defaultdict(list)
 
     def _contents_geq_value_validator(
         name: str, value: Union[float, int, Sequence], floor_value: Union[float, int]
     ) -> None:
@@ -216,15 +225,15 @@
         For Union[float, int], ensure the scalar is >= floor_value
         """
 
         # Do nothing for optional types
         if value is None:
             return
         elif isinstance(value, Sequence):
-            if not all([elem >= floor_value for elem in value]):
+            if not all(elem >= floor_value for elem in value):
                 raise ValueError(
                     f"`IPUConfig` attribute `{name}` must have all elements >= {floor_value}. You provided {value=}"
                 )
         elif isinstance(value, (int, float)):
             if not value >= floor_value:
                 raise ValueError(f"`IPUConfig` attribute `{name}` must be >= {floor_value}. You provided {value=}")
         else:
@@ -318,14 +327,17 @@
         recompute_checkpoint_every_layer: bool = False,
         device_iterations: int = 1,
         inference_device_iterations: int = 1,
         output_mode: str = "final",
         seed: Optional[int] = None,
         auto_loss_scaling: bool = False,
         executable_cache_dir: str = "",
+        explicit_ir_inference: bool = False,
+        parallelize_kwargs: Optional[Dict[str, Any]] = None,
+        inference_parallelize_kwargs: Optional[Dict[str, Any]] = None,
         **kwargs,
     ):
         self.seed = seed
 
         # Default mode to `training`
         self.train()
 
@@ -384,18 +396,22 @@
         self.device_iterations = device_iterations
         self.inference_device_iterations = inference_device_iterations
         self.optimizer_state_offchip = optimizer_state_offchip
         self.replicated_tensor_sharding = replicated_tensor_sharding
         self.auto_loss_scaling = auto_loss_scaling
         self.enable_half_partials = enable_half_partials
         self.executable_cache_dir = executable_cache_dir
+        self.explicit_ir_inference = explicit_ir_inference
         self.embedding_serialization_factor = embedding_serialization_factor
         self.recompute_checkpoint_every_layer = recompute_checkpoint_every_layer
         self.output_mode = output_mode
 
+        self.parallelize_kwargs = parallelize_kwargs or {}
+        self.inference_parallelize_kwargs = inference_parallelize_kwargs or {}
+
         # TODO: remove this if unnecessary.
         self.execute_encoder_on_cpu_for_generation = kwargs.pop("execute_encoder_on_cpu_for_generation", False)
 
         # Raise error if user has provided unknown & unused kwarg
         if unknown_kwargs := (set(kwargs) - set(BaseConfig().to_dict())):
             raise IncompatibleIPUConfigError(
                 "IPUConfig received unknown arguments:\n" + "\n".join([f"  {k}={kwargs[k]}" for k in unknown_kwargs])
@@ -644,14 +660,17 @@
 
         # Options for profiling with Popvision
         engine_options = {
             "opt.useAutoloader": "true",
             "target.syncReplicasIndependently": "true",
         }
 
+        if for_inference and self.explicit_ir_inference:
+            opts._popart.set("enableExplicitIR", True)
+
         opts._Popart.set("engineOptions", engine_options)
 
         self.mode = old_mode
         return opts
 
     def to_options(self, for_inference: bool = False, compile_only: bool = False) -> poptorch.Options:
         """
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/modelcard.py` & `optimum-graphcore-0.7.1/optimum/graphcore/modelcard.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/modeling_utils.py` & `optimum-graphcore-0.7.1/optimum/graphcore/modeling_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -799,7 +799,28 @@
     def forward(self, sequence, positions):
         """
         Gathers the vectors at the specific positions over a batch.
         """
         num_classes = int(sequence.shape[1])
         one_hot_positions = F.one_hot(positions, num_classes).to(dtype=sequence.dtype)
         return torch.matmul(one_hot_positions.detach(), sequence)
+
+
+def shift_tokens_right(input_ids: torch.Tensor, pad_token_id: int, decoder_start_token_id: int):
+    """
+    Shift input ids one token to the right.
+    """
+    # Upstream version:
+    # shifted_input_ids = input_ids.new_zeros(input_ids.shape)
+    # shifted_input_ids[:, 1:] = input_ids[:, :-1].clone()
+    # shifted_input_ids[:, 0] = decoder_start_token_id
+    # Change to fix slice assignment:
+    shifted_input_ids = torch.cat(
+        [torch.ones(input_ids.shape[0], 1, dtype=input_ids.dtype) * decoder_start_token_id, input_ids[:, :-1]], 1
+    )
+
+    if pad_token_id is None:
+        raise ValueError("self.model.config.pad_token_id has to be defined.")
+    # replace possible -100 values in labels by `pad_token_id`
+    shifted_input_ids = torch.where(shifted_input_ids == -100, pad_token_id, shifted_input_ids)
+
+    return shifted_input_ids
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/bart/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/bart/modeling_bart.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/bart/modeling_bart.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,27 +30,27 @@
 )
 from transformers.models.bart.modeling_bart import (
     BartAttention,
     BartDecoder,
     BartEncoder,
     BartEncoderLayer,
     BartLearnedPositionalEmbedding,
-    shift_tokens_right,
 )
 
 from optimum.utils import logging
 
 from ...generation import IPUAttentionMixin, IPUGenerationMixin, supports_kv_cache
 from ...modeling_utils import (
     PipelineMixin,
     SerializedLinear,
     SharedEmbedding,
     get_layer_ipu,
     recomputation_checkpoint,
     register,
+    shift_tokens_right,
     split_encoder_decoder_ipu_config,
 )
 
 
 logger = logging.get_logger(__name__)
 
 FLOAT16_LIMIT = 1e4
@@ -558,15 +558,15 @@
         original.__class__ = BartLearnedPositionalEmbedding
         return original
 
     def forward(self, input_ids: torch.Tensor, past_key_values_length: int = 0):
         if input_ids.shape[-1] == 1:
             # KV cache enabled.
             del past_key_values_length
-            return poptorch.dynamic_slice(self.weight, 0, self._generation_step + self.offset, 1, 1)
+            return torch.index_select(self.weight, 0, self._generation_step + self.offset)
         else:
             return super().forward(input_ids, past_key_values_length)
 
 
 class _BartModelWithSharedEmbedding(BartModel):
     @property
     def is_encoder_and_decoder_embeddings_computation_shared(self):
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/bert/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/bert/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .modeling_bert import (
+    PipelinedBertModel,
     PipelinedBertForMaskedLM,
     PipelinedBertForMultipleChoice,
     PipelinedBertForPreTraining,
     PipelinedBertForQuestionAnswering,
     PipelinedBertForSequenceClassification,
     PipelinedBertForTokenClassification,
 )
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/bert/bert_fused_attention.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/bert/bert_fused_attention.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/bert/modeling_bert.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/bert/modeling_bert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# Copyright 2018 The Google AI Language Team Authors and The HuggingFace Inc. team.
-# Copyright (c) 2018, NVIDIA CORPORATION.  All rights reserved.
-# Copyright (c) 2021 Graphcore Ltd. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,15 +24,15 @@
     BertForMultipleChoice,
     BertForPreTraining,
     BertForQuestionAnswering,
     BertForSequenceClassification,
     BertForTokenClassification,
 )
 from transformers.modeling_outputs import MaskedLMOutput, QuestionAnsweringModelOutput
-from transformers.models.bert.modeling_bert import BertForPreTrainingOutput, BertSelfAttention
+from transformers.models.bert.modeling_bert import BertForPreTrainingOutput, BertModel, BertSelfAttention
 
 from optimum.utils import logging
 
 from ...modeling_utils import (
     OnehotGather,
     PipelineMixin,
     SerializedEmbedding,
@@ -46,14 +44,74 @@
 )
 from .bert_fused_attention import BertFusedSelfAttention
 
 
 logger = logging.get_logger(__name__)
 
 
+@register(BertModel)
+class PipelinedBertModel(BertModel, PipelineMixin):
+    def __init__(self, config):
+        super().__init__(config)
+
+    def parallelize(self):
+        """
+        Transform the model to run in an IPU pipeline.
+        - Adds pipeline stages to the model
+        - Replaces self-attention layers with fused-qkv self-attention layers
+        - (If enabled) Replaces the word embedding with a SerializedEmbedding
+        - Adds recomputation checkpoints
+        """
+        super().parallelize()
+
+        # Use faster fused-qkv self-attention
+        for layer in self.encoder.layer:
+            layer.attention.self.__class__ = BertFusedSelfAttention
+
+        logger.info("-------------------- Device Allocation --------------------")
+        logger.info("Embedding --> IPU 0")
+        if self.ipu_config.embedding_serialization_factor > 1:
+            self.embeddings.word_embeddings = SerializedEmbedding.from_model(
+                self.embeddings.word_embeddings, self.ipu_config.embedding_serialization_factor
+            )
+        self.embeddings = poptorch.BeginBlock(self.embeddings, "Embedding", ipu_id=0)
+        hs = outline_attribute(self.embeddings.LayerNorm, "embedding")
+        self._hooks.extend(hs)
+
+        layer_ipu = get_layer_ipu(self.ipu_config, self.encoder.layer)
+        for index, layer in enumerate(self.encoder.layer):
+            ipu = layer_ipu[index]
+            if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_hidden_layers - 1:
+                h = recomputation_checkpoint(layer)
+                self._hooks.append(h)
+            self.encoder.layer[index] = poptorch.BeginBlock(layer, f"Encoder{index}", ipu_id=ipu)
+            logger.info(f"Encoder {index:<2} --> IPU {ipu}")
+
+        logger.info("Pooler --> IPU 0")
+        self.pooler = poptorch.BeginBlock(self.pooler, "Pooler", ipu_id=0)
+
+        return self
+
+    def deparallelize(self):
+        """
+        Undo the changes to the model done by `parallelize`.
+        You should call this before doing `save_pretrained` so that the `model.state_dict` is
+        compatible with the original model.
+        """
+        super().deparallelize()
+
+        for layer in self.encoder.layer:
+            layer.attention.self.__class__ = BertSelfAttention
+
+        # Deserialize the serialized word embedding
+        if self.ipu_config.embedding_serialization_factor > 1:
+            self.embeddings.word_embeddings = self.embeddings.word_embeddings.to_model()
+        return self
+
+
 @register(BertForPreTraining)
 class PipelinedBertForPreTraining(BertForPreTraining, PipelineMixin):
     """
     BertForPretraining transformed to run in an IPU pipeline.
 
     Recommended usage:
     ```
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/modeling_convnext.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/convnext/modeling_convnext.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/optimized_convnextlayer.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/convnext/optimized_convnextlayer.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/deberta/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/deberta/modeling_deberta.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/deberta/modeling_deberta.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/distilbert/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/distilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/distilbert/modeling_distilbert.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/distilbert/modeling_distilbert.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/modeling_gpt2.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/gpt2/modeling_gpt2.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/optimized_gpt2_attn.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/gpt2/optimized_gpt2_attn.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_attention.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/groupbert_attention.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_convolution.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/groupbert_convolution.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_ffn.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/groupbert_ffn.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/modeling_groupbert.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/groupbert/modeling_groupbert.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/hubert/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/ipu_layer_drop.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/hubert/ipu_layer_drop.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/modeling_hubert.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/hubert/modeling_hubert.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/lxmert/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/lxmert/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/lxmert/modeling_lxmert.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/lxmert/modeling_lxmert.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/mt5/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/mt5/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/mt5/modeling_mt5.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/mt5/modeling_mt5.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/roberta/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/roberta/modeling_roberta.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/roberta/modeling_roberta.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/t5/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/t5/configuration_t5.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/t5/configuration_t5.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/t5/modeling_t5.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/whisper/modeling_whisper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,569 +1,705 @@
-#  Copyright 2022 The HuggingFace Team. All rights reserved.
-#  Copyright (c) 2022 Graphcore Ltd. All rights reserved.
+# Copyright 2022 The OpenAI Authors and The HuggingFace Inc. team. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-import warnings
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+import copy
 from typing import Optional, Tuple, Union
 
 import poptorch
 import torch
-import torch.nn as nn
-from torch import Tensor
-from transformers import T5ForConditionalGeneration
-from transformers.activations import NewGELUActivation
+from torch import nn
 from transformers.modeling_outputs import BaseModelOutput, Seq2SeqLMOutput
-from transformers.models.t5.modeling_t5 import __HEAD_MASK_WARNING_MSG, T5Block, T5EncoderModel, T5Stack
+from transformers.models.whisper.modeling_whisper import (
+    WhisperAttention,
+    WhisperDecoder,
+    WhisperEncoder,
+    WhisperEncoderLayer,
+    WhisperForConditionalGeneration,
+    WhisperPositionalEmbedding,
+)
 
 from optimum.utils import logging
 
-from ...generation import IPUGenerationMixin
+from ...generation import IPUAttentionMixin, IPUGenerationMixin, assert_poptorch_supports_cond, supports_kv_cache
 from ...modeling_utils import (
     PipelineMixin,
     SerializedLinear,
-    SharedEmbedding,
     get_layer_ipu,
     recomputation_checkpoint,
     register,
+    shift_tokens_right,
     split_encoder_decoder_ipu_config,
 )
 
 
 logger = logging.get_logger(__name__)
 
 
-class UpCastWrapper(nn.Module):
-    def __init__(self, module: nn.Module, scale: float = 1.0):
-        super().__init__()
-        self.module = module
-        self.scale = scale
-
-    def forward(self, input):
-        return self.module(input).to(torch.float32) * self.scale
-
-
-class CustomGELU(NewGELUActivation):
-    # Work-around bug with torch.nn.GELU(approximate="tanh")
-    # TODO: Remove this when bug is fixed
-    def forward(self, input: Tensor) -> Tensor:
-        safe = torch.logical_and(-39 < input, input < 39)
-        safe_input = torch.where(safe, input, 0.0)
-        gelu = super().forward(safe_input)
-        relu = nn.functional.relu(input)
-        return torch.where(safe, gelu, relu)
+FLOAT16_LIMIT = 1e4
+
+
+# Copied from transformers.models.bart.modeling_bart._make_causal_mask
+def _make_causal_mask(input_ids_shape: torch.Size, dtype: torch.dtype, past_key_values_length: int = 0):
+    """
+    Make causal mask used for bi-directional self-attention.
+    """
+    bsz, tgt_len = input_ids_shape
+    mask = torch.full((tgt_len, tgt_len), -FLOAT16_LIMIT)
+    mask_cond = torch.arange(mask.size(-1))
+    mask.masked_fill_(mask_cond < (mask_cond + 1).view(mask.size(-1), 1), 0)
+    mask = mask.to(dtype)
+
+    if past_key_values_length > 0:
+        mask = torch.cat([torch.zeros(tgt_len, past_key_values_length, dtype=dtype), mask], dim=-1)
+    return mask[None, None, :, :].expand(bsz, 1, tgt_len, tgt_len + past_key_values_length)
+
+
+# Copied from transformers.models.bart.modeling_bart._expand_mask
+def _expand_mask(mask: torch.Tensor, dtype: torch.dtype, tgt_len: Optional[int] = None):
+    """
+    Expands attention_mask from `[bsz, seq_len]` to `[bsz, 1, tgt_seq_len, src_seq_len]`.
+    """
+    bsz, src_len = mask.size()
+    tgt_len = tgt_len if tgt_len is not None else src_len
+
+    expanded_mask = mask[:, None, None, :].expand(bsz, 1, tgt_len, src_len).to(dtype)
+
+    inverted_mask = 1.0 - expanded_mask
+
+    return inverted_mask.masked_fill(inverted_mask.to(torch.bool), -FLOAT16_LIMIT)
 
 
-class CustomT5Block(T5Block):
+class IPUWhisperAttention(WhisperAttention, IPUAttentionMixin):
     def forward(
         self,
-        hidden_states,
-        attention_mask=None,
-        position_bias=None,
-        encoder_hidden_states=None,
-        encoder_attention_mask=None,
-        encoder_decoder_position_bias=None,
-        layer_head_mask=None,
-        cross_attn_layer_head_mask=None,
-        past_key_value=None,
-        use_cache=False,
-        output_attentions=False,
-        return_dict=True,
-    ):
-        if past_key_value is not None:
-            if not self.is_decoder:
-                logger.warning("`past_key_values` is passed to the encoder. Please make sure this is intended.")
-            expected_num_past_key_values = 2 if encoder_hidden_states is None else 4
+        hidden_states: torch.Tensor,
+        key_value_states: Optional[torch.Tensor] = None,
+        past_key_value: Optional[Tuple[torch.Tensor]] = None,
+        attention_mask: Optional[torch.Tensor] = None,
+        layer_head_mask: Optional[torch.Tensor] = None,
+        output_attentions: bool = False,
+    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
+        bsz, tgt_len, _ = hidden_states.size()
+
+        query_states = self.q_proj(hidden_states) * self.scaling
+        if key_value_states is not None:
+            if self.cross_kv_cache_initialized:
+                # cross attention with cross kv cache
+                key_states, value_states = self.add_to_cross_kv_cache(
+                    key_value_states,
+                    lambda x: self._shape(self.k_proj(x), -1, bsz),
+                    lambda x: self._shape(self.v_proj(x), -1, bsz),
+                )
+            else:
+                # cross attention
+                key_states = self._shape(self.k_proj(key_value_states), -1, bsz)
+                value_states = self._shape(self.v_proj(key_value_states), -1, bsz)
+        elif self.kv_cache_initialized:
+            # self attention with kv cache
+            key_states = self._shape(self.k_proj(hidden_states), -1, bsz)
+            value_states = self._shape(self.v_proj(hidden_states), -1, bsz)
+
+            if tgt_len != 1:
+                raise ValueError(f"KV cache expects tgt_len = 1, received {tgt_len}.")
+
+            key_states, value_states = self.add_to_kv_cache(key_states, value_states)
+            attention_mask = self.update_attention_mask(attention_mask)
+        else:
+            # self attention
+            key_states = self._shape(self.k_proj(hidden_states), -1, bsz)
+            value_states = self._shape(self.v_proj(hidden_states), -1, bsz)
+
+        if self.is_decoder:
+            # We handle the KV cache via buffers, not via the eager approach of passing the cache around.
+            # This is retained so upstream DecoderLayer can stay as is and that tests pass.
+            past_key_value = (key_states, value_states)
+
+        proj_shape = (bsz * self.num_heads, -1, self.head_dim)
+        query_states = self._shape(query_states, tgt_len, bsz).view(*proj_shape)
+        key_states = key_states.reshape(*proj_shape)
+        value_states = value_states.reshape(*proj_shape)
+
+        src_len = key_states.size(1)
+
+        # Change: optionally serialize attention, mainly intended for the encoder with large sequence length.
+        if self.is_attention_serialized:
+            if layer_head_mask is not None:
+                raise ValueError("layer_head_mask is not supported yet with serialized attention.")
+
+            if self.dropout or self.training:
+                raise ValueError("dropout is not supported yet with serialized attention.")
+
+            if attention_mask is not None:
+                if attention_mask.size() != (bsz, 1, tgt_len, src_len):
+                    raise ValueError(
+                        f"Attention mask should be of size {(bsz, 1, tgt_len, src_len)}, but is {attention_mask.size()}"
+                    )
+                attention_mask = attention_mask.view(bsz, tgt_len, src_len).repeat(self.num_heads, 1, 1)
+
+            attn_output = self.serialized_attention(query_states, key_states, value_states, 1.0, attention_mask)
+        else:
+            attn_weights = torch.bmm(query_states, key_states.transpose(1, 2))
 
-            if len(past_key_value) != expected_num_past_key_values:
+            if attn_weights.size() != (bsz * self.num_heads, tgt_len, src_len):
                 raise ValueError(
-                    f"There should be {expected_num_past_key_values} past states. "
-                    f"{'2 (past / key) for cross attention. ' if expected_num_past_key_values == 4 else ''}"
-                    f"Got {len(past_key_value)} past key / value states"
+                    f"Attention weights should be of size {(bsz * self.num_heads, tgt_len, src_len)}, but is"
+                    f" {attn_weights.size()}"
                 )
 
-            self_attn_past_key_value = past_key_value[:2]
-            cross_attn_past_key_value = past_key_value[2:]
-        else:
-            self_attn_past_key_value, cross_attn_past_key_value = None, None
+            if attention_mask is not None:
+                if attention_mask.size() != (bsz, 1, tgt_len, src_len):
+                    raise ValueError(
+                        f"Attention mask should be of size {(bsz, 1, tgt_len, src_len)}, but is {attention_mask.size()}"
+                    )
+                attn_weights = attn_weights.view(bsz, self.num_heads, tgt_len, src_len) + attention_mask
+                attn_weights = attn_weights.view(bsz * self.num_heads, tgt_len, src_len)
+
+            attn_weights = nn.functional.softmax(attn_weights, dim=-1)
+
+            if layer_head_mask is not None:
+                if layer_head_mask.size() != (self.num_heads,):
+                    raise ValueError(
+                        f"Head mask for a single layer should be of size {(self.num_heads,)}, but is"
+                        f" {layer_head_mask.size()}"
+                    )
+                attn_weights = layer_head_mask.view(1, -1, 1, 1) * attn_weights.view(
+                    bsz, self.num_heads, tgt_len, src_len
+                )
+                attn_weights = attn_weights.view(bsz * self.num_heads, tgt_len, src_len)
+
+            # Change: delete optional reshaping of attn_weights
+
+            attn_probs = nn.functional.dropout(attn_weights, p=self.dropout, training=self.training)
+
+            attn_output = torch.bmm(attn_probs, value_states)
+
+        if attn_output.size() != (bsz * self.num_heads, tgt_len, self.head_dim):
+            raise ValueError(
+                f"`attn_output` should be of size {(bsz, self.num_heads, tgt_len, self.head_dim)}, but is"
+                f" {attn_output.size()}"
+            )
+
+        attn_output = attn_output.view(bsz, self.num_heads, tgt_len, self.head_dim)
+        attn_output = attn_output.transpose(1, 2)
+
+        attn_output = attn_output.reshape(bsz, tgt_len, self.embed_dim)
+        attn_output = self.out_proj(attn_output)
 
-        self_attention_outputs = self.layer[0](
-            hidden_states,
+        # Change: modified check for output_attentions
+        if not output_attentions:
+            attn_weights = None
+
+        return attn_output, attn_weights, past_key_value
+
+
+class _WhisperEncoderLayerClamp(nn.Module):
+    def forward(
+        self,
+        hidden_states: torch.Tensor,
+        attention_mask: torch.Tensor,
+        layer_head_mask: torch.Tensor,
+        output_attentions: bool = False,
+    ):
+        """
+        Args:
+            hidden_states (`torch.FloatTensor`): input to the layer of shape `(batch, seq_len, embed_dim)`
+            attention_mask (`torch.FloatTensor`): attention mask of size
+                `(batch, 1, tgt_len, src_len)` where padding elements are indicated by very large negative values.
+            layer_head_mask (`torch.FloatTensor`): mask for attention heads in a given layer of size
+                `(config.encoder_attention_heads,)`.
+            output_attentions (`bool`, *optional*):
+                Whether or not to return the attentions tensors of all attention layers. See `attentions` under
+                returned tensors for more detail.
+        """
+        residual = hidden_states
+        hidden_states = self.self_attn_layer_norm(hidden_states)
+        hidden_states, attn_weights, _ = self.self_attn(
+            hidden_states=hidden_states,
             attention_mask=attention_mask,
-            position_bias=position_bias,
             layer_head_mask=layer_head_mask,
-            past_key_value=self_attn_past_key_value,
-            use_cache=use_cache,
             output_attentions=output_attentions,
         )
-        hidden_states, present_key_value_state = self_attention_outputs[:2]
-        attention_outputs = self_attention_outputs[2:]  # Keep self-attention outputs and relative position weights
-
-        # clamp inf values to enable fp16 training
-        # Custom: Remove check for inf
-        if hidden_states.dtype == torch.float16:
-            clamp_value = torch.tensor(torch.finfo(hidden_states.dtype).max - 1000, dtype=hidden_states.dtype)
-            hidden_states = torch.clamp(hidden_states, min=-clamp_value, max=clamp_value)
-
-        do_cross_attention = self.is_decoder and encoder_hidden_states is not None
-        if do_cross_attention:
-            # the actual query length is unknown for cross attention
-            # if using past key value states. Need to inject it here
-            if present_key_value_state is not None:
-                query_length = present_key_value_state[0].shape[2]
-            else:
-                query_length = None
+        hidden_states = nn.functional.dropout(hidden_states, p=self.dropout, training=self.training)
+        hidden_states = residual + hidden_states
 
-            cross_attention_outputs = self.layer[1](
-                hidden_states,
-                key_value_states=encoder_hidden_states,
-                attention_mask=encoder_attention_mask,
-                position_bias=encoder_decoder_position_bias,
-                layer_head_mask=cross_attn_layer_head_mask,
-                past_key_value=cross_attn_past_key_value,
-                query_length=query_length,
-                use_cache=use_cache,
-                output_attentions=output_attentions,
-            )
-            hidden_states = cross_attention_outputs[0]
+        residual = hidden_states
+        hidden_states = self.final_layer_norm(hidden_states)
+        hidden_states = self.activation_fn(self.fc1(hidden_states))
+        hidden_states = nn.functional.dropout(hidden_states, p=self.activation_dropout, training=self.training)
+        hidden_states = self.fc2(hidden_states)
+        hidden_states = nn.functional.dropout(hidden_states, p=self.dropout, training=self.training)
+        hidden_states = residual + hidden_states
+
+        # NOTE: This differs from the original implementation
+        # There is a type mismatch bug with this call to clamp so we remove it here. It is anyway not needed on IPU because FP16 values are clamped to maximum value by default.
+        # TODO: when bug is fixed in future SDK remove this entire class;
 
-            # clamp inf values to enable fp16 training
-            # Custom: Remove check for inf
-            if hidden_states.dtype == torch.float16:
-                clamp_value = torch.tensor(torch.finfo(hidden_states.dtype).max - 1000, dtype=hidden_states.dtype)
-                hidden_states = torch.clamp(hidden_states, min=-clamp_value, max=clamp_value)
-
-            # Combine self attn and cross attn key value states
-            if present_key_value_state is not None:
-                present_key_value_state = present_key_value_state + cross_attention_outputs[1]
-
-            # Keep cross-attention outputs and relative position weights
-            attention_outputs = attention_outputs + cross_attention_outputs[2:]
-
-        # Apply Feed Forward layer
-        hidden_states = self.layer[-1](hidden_states)
-
-        # clamp inf values to enable fp16 training
-        # Custom: Remove check for inf
-        if hidden_states.dtype == torch.float16:
-            clamp_value = torch.tensor(torch.finfo(hidden_states.dtype).max - 1000, dtype=hidden_states.dtype)
-            hidden_states = torch.clamp(hidden_states, min=-clamp_value, max=clamp_value)
+        # clamp_value = torch.finfo(hidden_states.dtype).max - 1000
+        # hidden_states = torch.clamp(hidden_states, min=-clamp_value, max=clamp_value)
 
         outputs = (hidden_states,)
 
-        if use_cache:
-            outputs = outputs + (present_key_value_state,) + attention_outputs
+        if output_attentions:
+            outputs += (attn_weights,)
+
+        return outputs
+
+
+class IPUWhisperPositionalEmbedding(WhisperPositionalEmbedding):
+    @classmethod
+    def from_model(cls, model: WhisperPositionalEmbedding):
+        clone = copy.deepcopy(model)
+        clone.__class__ = cls
+        clone.register_buffer("_generation_step", torch.tensor([0], dtype=torch.int32), persistent=False)
+        return clone
+
+    def to_model(self) -> WhisperPositionalEmbedding:
+        del self._generation_step
+
+        original = copy.deepcopy(self)
+        original.__class__ = WhisperPositionalEmbedding
+        return original
+
+    def forward(self, input_ids: torch.Tensor, past_key_values_length: int = 0):
+        if input_ids.shape[-1] == 1:
+            # KV cache enabled.
+            del past_key_values_length
+            return torch.index_select(self.weight, 0, self._generation_step)
         else:
-            outputs = outputs + attention_outputs
+            return super().forward(input_ids, past_key_values_length=past_key_values_length)
 
-        return outputs  # hidden-states, present_key_value_states, (self-attention position bias), (self-attention weights), (cross-attention position bias), (cross-attention weights)
 
+class _WhisperDecoderWithCustomMakeCausalAndExpandMask(WhisperDecoder):
+    """
+    Transformer decoder consisting of *config.decoder_layers* layers. Each layer is a [`WhisperDecoderLayer`]
+
+    Args:
+        config: WhisperConfig
+    """
+
+    def _prepare_decoder_attention_mask(self, attention_mask, input_shape, inputs_embeds, past_key_values_length):
+        # create causal mask
+        # [bsz, seq_len] -> [bsz, 1, tgt_seq_len, src_seq_len]
+        combined_attention_mask = None
+
+        if input_shape[-1] > 1:
+            combined_attention_mask = _make_causal_mask(
+                input_shape, inputs_embeds.dtype, past_key_values_length=past_key_values_length
+            ).to(inputs_embeds.device)
+
+        if attention_mask is not None:
+            # [bsz, seq_len] -> [bsz, 1, tgt_seq_len, src_seq_len]
+            expanded_attn_mask = _expand_mask(attention_mask, inputs_embeds.dtype, tgt_len=input_shape[-1])
+            combined_attention_mask = (
+                expanded_attn_mask if combined_attention_mask is None else expanded_attn_mask + combined_attention_mask
+            )
+
+        return combined_attention_mask
+
+
+class IPUWhisperConditionalEncoder(WhisperEncoder):
+    @classmethod
+    def from_model(cls, model: WhisperEncoder, batch_size: int, num_beams: int):
+        clone = model
+        clone.__class__ = cls
+        clone.register_buffer(
+            "_encoder_last_hidden_state",
+            torch.zeros((batch_size, model.config.max_source_positions, model.config.d_model), dtype=model.dtype),
+            persistent=False,
+        )
+        clone.register_buffer("_generation_step", torch.tensor([0], dtype=torch.int32), persistent=False)
+        clone._batch_size = batch_size
+        clone._num_beams = num_beams
+        return clone
+
+    def to_model(self) -> WhisperEncoder:
+        del self._encoder_last_hidden_state
+        del self._generation_step
+        del self._batch_size
+        del self._num_beams
+
+        original = self
+        original.__class__ = WhisperEncoder
+        return original
+
+    def forward(
+        self,
+        input_features,
+        attention_mask=None,
+        head_mask=None,
+        output_attentions=None,
+        output_hidden_states=None,
+        return_dict=None,
+    ):
+        if attention_mask is not None or head_mask is not None or output_attentions or output_hidden_states:
+            raise ValueError(f"{self.__class__.__name__} only accepts `input_features`.")
 
-class CustomT5Stack(T5Stack):
-    def invert_attention_mask(self, *args, **kwargs) -> Tensor:
-        return super().invert_attention_mask(*args, **kwargs) * 0.75
+        def run_encoder(input_features):
+            encoder_output = WhisperEncoder.forward(self, input_features, return_dict=True)
+            return encoder_output.last_hidden_state
 
-    def get_extended_attention_mask(self, *args, **kwargs) -> Tensor:
-        return super().get_extended_attention_mask(*args, **kwargs) * 0.75
+        def skip_encoder(input_features):
+            return self._encoder_last_hidden_state
 
+        self._encoder_last_hidden_state.copy_(
+            poptorch.cond(self._generation_step == 0, run_encoder, [input_features], skip_encoder, [input_features])[0]
+        )
+        last_hidden_state = self._encoder_last_hidden_state
+        if self._num_beams > 1:
+            # Before being passed to the decoder, we must expand the encoder outputs when beam search is enabled
+            # as this would be done on host.
+            last_hidden_state = last_hidden_state.repeat_interleave(
+                self._num_beams, dim=0, output_size=self._batch_size * self._num_beams
+            )
+        return BaseModelOutput(last_hidden_state=last_hidden_state)
 
-@register(T5ForConditionalGeneration)
-class PipelinedT5ForConditionalGeneration(T5ForConditionalGeneration, PipelineMixin, IPUGenerationMixin):
-    @property
-    def is_encoder_and_decoder_embeddings_computation_shared(self):
-        return isinstance(self.shared, SharedEmbedding)
 
-    def encoder_and_decoder_embeddings_computation(self, use_shared_embedding: bool):
-        """Sets the T5ForConditionalGeneration shared embedding layer to SharedEmbedding that combines the computation under one layer.
+@supports_kv_cache
+@register(WhisperForConditionalGeneration)
+class PipelinedWhisperForConditionalGeneration(WhisperForConditionalGeneration, PipelineMixin, IPUGenerationMixin):
+    def change_encoder_layer_class(self, restore: bool):
+        """Changes the encoder layer class to avoid the dynamic 'if'
 
         Args:
-            use_shared_embedding: whether to use SharedEmbedding or not.
+            restore: whether to restore the encoder layers to their original version or not.
         """
+        for layer in self.model.encoder.layers:
+            layer.__class__ = WhisperEncoderLayer if restore else _WhisperEncoderLayerClamp
 
-        if use_shared_embedding:
-            if isinstance(self.shared, SharedEmbedding):
-                logger.warning("encoder and decoder embeddings computation is already shared")
-            else:
-                self.shared = SharedEmbedding(self.shared)
+    def change_encoder_class(self, restore: bool, **kwargs):
+        """Changes the encoder class to run the encoder under a `poptorch.cond` op.
+
+        Args:
+            restore: whether to restore the encoder to its original version or not.
+        """
+        batch_size = kwargs.get("batch_size", 1)
+        num_beams = kwargs.get("num_beams", 1)
+        encoder = self.model.get_encoder()
+        if restore:
+            if isinstance(encoder, IPUWhisperConditionalEncoder):
+                self.model.encoder = encoder.to_model()
         else:
-            if isinstance(self.shared, nn.Embedding):
-                logger.warning("encoder and decoder embeddings computation is not shared")
-            else:
-                self.shared = self.shared.shared
+            if self.ipu_config.inference_ipus_per_replica > 1:
+                raise ValueError(
+                    f"`{self.ipu_config.inference_ipus_per_replica=}` should be 1 when placing encoder and decoder on the same IPU."
+                )
+            assert_poptorch_supports_cond(
+                context="Whisper encoder is being conditionally run on the same IPU as the decoder since `use_cond_encoder=True`."
+            )
+            self.model.encoder = IPUWhisperConditionalEncoder.from_model(encoder, batch_size, num_beams)
+
+    def change_decoder_class(self, restore: bool):
+        """Changes the decoder class to update the _prepare_decoder_attention_mask method.
 
-    def parallelize(self, for_generation=False):
+        Args:
+            restore: whether to restore the decoder to its original version or not.
         """
-        Transform the model to run in an IPU pipeline.
-        - Adds pipeline stages to the model
-        - (If enabled) Replaces the shared embedding with a SerializedEmbedding
-        - Adds recomputation checkpoints
-
-        Recommended usage:
-        ```
-        model = PipelinedT5ForConditionalGeneration(config).parallelize().half()
-        ```
+        self.model.decoder.__class__ = WhisperDecoder if restore else _WhisperDecoderWithCustomMakeCausalAndExpandMask
+
+    def change_decoder_positional_embedding(self, restore: bool):
+        """Changes the decoder positional embedding to support an optional static KV cache.
+
+        Args:
+            restore: whether to restore the decoder positional embedding to their original version or not.
+        """
+        position_embedding = self.model.decoder.embed_positions
+        self.model.decoder.embed_positions = (
+            position_embedding.to_model() if restore else IPUWhisperPositionalEmbedding.from_model(position_embedding)
+        )
+
+    def change_attention_class(self, restore=False, **kwargs):
+        """Change the attention layers to support a KV cache.
+
+        Args:
+            restore: whether to restore the attention layers to their original version or not.
         """
-        PipelineMixin.parallelize(self)
+        batch_size = kwargs.get("batch_size", 1)
+        num_beams = kwargs.get("num_beams", 1)
+        use_cache = kwargs.get("use_cache", False)
+        max_length = kwargs.get("max_length", 448)
+        use_cross_cache = kwargs.get("use_cross_cache", False)
+        encoder_max_length = kwargs.get("encoder_max_length", 1500)
+        batch_serialization_factor = kwargs.get("batch_serialization_factor", 1)
+        sequence_serialization_factor = kwargs.get("sequence_serialization_factor", 1)
+
+        for encoder_layer in self.model.encoder.layers:
+            if restore:
+                encoder_layer.self_attn = encoder_layer.self_attn.to_model(WhisperAttention)
+                continue
+
+            encoder_layer.self_attn = IPUWhisperAttention.from_model(
+                encoder_layer.self_attn,
+                use_cache=False,
+                batch_serialization_factor=batch_serialization_factor,
+                sequence_serialization_factor=sequence_serialization_factor,
+            )
+
+        for decoder_layer in self.model.decoder.layers:
+            if restore:
+                decoder_layer.self_attn = decoder_layer.self_attn.to_model(WhisperAttention)
+                decoder_layer.encoder_attn = decoder_layer.encoder_attn.to_model(WhisperAttention)
+                continue
 
-        logger.info("-------------------- Device Allocation --------------------")
-        logger.info("Embedding  --> IPU 0")
+            decoder_layer.self_attn = IPUWhisperAttention.from_model(
+                decoder_layer.self_attn,
+                use_cache=use_cache,
+                use_cross_cache=False,
+                batch_size=batch_size,
+                max_length=max_length,
+                num_beams=num_beams,
+                dtype=decoder_layer.self_attn.k_proj.weight.dtype,
+            )
+            decoder_layer.encoder_attn = IPUWhisperAttention.from_model(
+                decoder_layer.encoder_attn,
+                use_cache=False,
+                use_cross_cache=use_cross_cache,
+                batch_size=batch_size,
+                encoder_max_length=encoder_max_length,
+                num_beams=num_beams,
+                dtype=decoder_layer.encoder_attn.k_proj.weight.dtype,
+            )
 
-        if self.ipu_config.embedding_serialization_factor > 1:
-            self.lm_head = SerializedLinear.from_model(self.lm_head, self.ipu_config.embedding_serialization_factor)
-            # TODO: is it needed to check?
-            if self.config.tie_word_embeddings:
+    def change_lm_head(self, restore: bool, use_cache: bool = None):
+        # Maybe use _IndexedInputLinear
+        self.change_lm_head_to_indexed_input_linear(restore or use_cache)
+        # Maybe use SerializedLinear
+        if restore:
+            lm_head = self.get_output_embeddings()
+            if isinstance(lm_head, SerializedLinear):
+                self.set_output_embeddings(lm_head.to_model())
                 self.tie_weights()
+        else:
+            projection_serialization_factor = max(
+                self.ipu_config._projection_serialization_factor or 1,
+                sum(self.ipu_config._serialized_projection_splits_per_ipu or [1]),
+            )
+            if projection_serialization_factor > 1:
+                self.set_output_embeddings(
+                    SerializedLinear.from_model(self.get_output_embeddings(), projection_serialization_factor)
+                )
+                self.tie_weights()
+
+    def quantize_linear_layers(self, restore: bool, num_groups: int = 16):
+        if not restore:
+            from ...quantization.group_quantize import GroupQuantLinear
+
+            logger.info("Group quantizing linear layers")
+            for module in self.model.encoder.layers:
+                module.self_attn.q_proj = GroupQuantLinear.from_model(module.self_attn.q_proj, num_groups)
+                module.self_attn.k_proj = GroupQuantLinear.from_model(module.self_attn.k_proj, num_groups)
+                module.self_attn.v_proj = GroupQuantLinear.from_model(module.self_attn.v_proj, num_groups)
+                module.self_attn.out_proj = GroupQuantLinear.from_model(module.self_attn.out_proj, num_groups)
+                module.fc1 = GroupQuantLinear.from_model(module.fc1, num_groups)
+                module.fc2 = GroupQuantLinear.from_model(module.fc2, num_groups)
+
+            for module in self.model.decoder.layers:
+                module.self_attn.q_proj = GroupQuantLinear.from_model(module.self_attn.q_proj, num_groups)
+                module.self_attn.k_proj = GroupQuantLinear.from_model(module.self_attn.k_proj, num_groups)
+                module.self_attn.v_proj = GroupQuantLinear.from_model(module.self_attn.v_proj, num_groups)
+                module.self_attn.out_proj = GroupQuantLinear.from_model(module.self_attn.out_proj, num_groups)
+                module.encoder_attn.q_proj = GroupQuantLinear.from_model(module.encoder_attn.q_proj, num_groups)
+                module.encoder_attn.k_proj = GroupQuantLinear.from_model(module.encoder_attn.k_proj, num_groups)
+                module.encoder_attn.v_proj = GroupQuantLinear.from_model(module.encoder_attn.v_proj, num_groups)
+                module.encoder_attn.out_proj = GroupQuantLinear.from_model(module.encoder_attn.out_proj, num_groups)
+                module.fc1 = GroupQuantLinear.from_model(module.fc1, num_groups)
+                module.fc2 = GroupQuantLinear.from_model(module.fc2, num_groups)
 
-        self.change_lm_head_to_indexed_input_linear(restore=not for_generation)
+    def parallelize(self, for_generation=False, use_cache=False, use_cross_cache=False, **kwargs):
+        super().parallelize()
+
+        if use_cache:
+            kwargs = self._populate_parallelize_kwargs_with_generation_config(**kwargs)
 
-        self.encoder_and_decoder_embeddings_computation(True)
-        self.shared = poptorch.BeginBlock(self.shared, "Embedding", ipu_id=0)
+        self._use_cond_encoder = kwargs.get("use_cond_encoder", False)
+        self._use_encoder_output_buffer = kwargs.get("use_encoder_output_buffer", False)
+        if self._use_cond_encoder and self._use_encoder_output_buffer:
+            raise ValueError(
+                "`use_cond_encoder=True` is incompatible with `use_encoder_output_buffer=True`, only set one to True."
+            )
+        self._use_group_quantized_linears = kwargs.get("use_group_quantized_linears", False)
+
+        self.change_encoder_layer_class(restore=False)
+        self.change_decoder_class(restore=False)
+        self.change_decoder_positional_embedding(restore=False)
+        self.change_attention_class(
+            restore=False,
+            use_cache=use_cache and for_generation,
+            use_cross_cache=use_cross_cache and for_generation,
+            **kwargs,
+        )
+        self.change_lm_head(restore=False, use_cache=use_cache or not for_generation)
+        self.change_encoder_class(restore=not self._use_cond_encoder, **kwargs)
+        self.quantize_linear_layers(restore=not self._use_group_quantized_linears, num_groups=16)
+        self.set_on_device_generation_steps(kwargs.get("on_device_generation_steps", 0))
+
+        logger.info("---------- Device Allocation -----------")
+        logger.info("conv1, conv2, embed_positions  --> IPU 0")
+        self.model.encoder.conv1 = poptorch.BeginBlock(self.model.encoder.conv1, "Conv1", ipu_id=0)
+        self.model.encoder.conv2 = poptorch.BeginBlock(self.model.encoder.conv2, "Conv2", ipu_id=0)
+        self.model.encoder.embed_positions = poptorch.BeginBlock(
+            self.model.encoder.embed_positions, "Embed Positions", ipu_id=0
+        )
 
-        # Use a custom T5Stack implementation because sharing the position bias causes OOM error
-        self.encoder.__class__ = CustomT5Stack
-        self.decoder.__class__ = CustomT5Stack
-
-        # Upcast input embeddings so that the residuals remain in FP32. This
-        # cast is reversed where necessary by the T5LayerNorm layers in:
-        # - first layer of T5LayerSelfAttention
-        # - first layer of T5LayerFF
-        # - final_layer_norm
-        # Which, conveniently, are all the places that this needs to happen.
-        # Therefore, so we just need to upcast immediately before the residual
-        # adds in T5LayerSelfAttention and T5LayerFF. This is handled in the
-        # for loop below.
-        self.encoder.embed_tokens = UpCastWrapper(self.encoder.embed_tokens)
-
-        # Use a custom T5Block implementation that removes a dynamic if blocks that can't be statically traced
-        for block in self.encoder.block:
-            block.__class__ = CustomT5Block
-            # Dropout happens immediately before the residual add. Inserting a
-            # cast in T5LayerSelfAttention and T5LayerFF keeps the residual
-            # structure in FP32
-            block.layer[0].dropout = UpCastWrapper(block.layer[0].dropout)
-            # Scale down the weights for the T5LayerFF down-projection and
-            # then scale its output back up again after it is cast to FP32
-            scale = 8.0
-            with torch.no_grad():
-                block.layer[1].DenseReluDense.wo.weight /= scale
-            block.layer[1].dropout = UpCastWrapper(block.layer[1].dropout, scale)
-            # Prevent overflow in NewGELUActivation
-            if self.config.dense_act_fn == "gelu_new":
-                # TODO: Work-around bug with torch.nn.GELU(approximate="tanh"). Replace
-                # this with block.layer[1].DenseReluDense.act = torch.nn.GELU(approximate="tanh")
-                # when bug is fixed
-                block.layer[1].DenseReluDense.act = CustomGELU()
-        for block in self.decoder.block:
-            block.__class__ = CustomT5Block
-            # Work-around bug with torch.nn.GELU(approximate="tanh")
-            # TODO: Remove this when bug is fixed
-            if self.config.dense_act_fn == "gelu_new":
-                block.layer[2].DenseReluDense.act = CustomGELU()
-
-        num_encoder_layers = len(self.encoder.block)
-        num_decoder_layers = len(self.decoder.block)
-
-        if for_generation:
-            # If running for text generation we split the IPU config into two configs
-            # because we run the encoder and decoder as separate Poplar executors.
+        num_encoder_layers = len(self.model.encoder.layers)
+        num_decoder_layers = len(self.model.decoder.layers)
+
+        if for_generation and not self._use_cond_encoder:
+            # If running for text generation (and the encoder and decoder are run as separate Poplar executors)
+            # we split the IPU config into two configs.
             ipu_configs = split_encoder_decoder_ipu_config(self.ipu_config, num_encoder_layers, num_decoder_layers)
             self.encoder_ipu_config, self.decoder_ipu_config = ipu_configs
             encoder_layer_ipu = get_layer_ipu(self.encoder_ipu_config, num_encoder_layers)
             decoder_layer_ipu = get_layer_ipu(self.decoder_ipu_config, num_decoder_layers)
         else:
             number_of_layers = num_encoder_layers + num_decoder_layers
             layer_ipu = get_layer_ipu(self.ipu_config, number_of_layers)
             encoder_layer_ipu = layer_ipu[:num_encoder_layers]
             decoder_layer_ipu = layer_ipu[num_encoder_layers:]
 
-        for index, (layer, ipu) in enumerate(zip(self.encoder.block, encoder_layer_ipu)):
-            if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_layers - 1:
+        for index, (layer, ipu) in enumerate(zip(self.model.encoder.layers, encoder_layer_ipu)):
+            if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_hidden_layers - 1:
                 self._hooks.append(recomputation_checkpoint(layer))
-            self.encoder.block[index] = poptorch.BeginBlock(layer, f"Encoder{index}", ipu_id=ipu)
+            self.model.encoder.layers[index] = poptorch.BeginBlock(layer, f"Encoder{index}", ipu_id=ipu)
             logger.info(f"Encoder {index:<2} --> IPU {ipu}")
 
-        self.encoder.final_layer_norm = poptorch.BeginBlock(
-            self.encoder.final_layer_norm, "Encoder Stack Final LayerNorm", ipu_id=ipu
+        # we need to deal with the model.encoder.layer norm
+        self.model.encoder.layer_norm = poptorch.BeginBlock(
+            self.model.encoder.layer_norm, "Encoder Layer Norm", ipu_id=ipu
+        )
+        logger.info(f"Encoder LN --> IPU {ipu}")
+
+        decoder_embedding_ipu = decoder_layer_ipu[0]
+        if (serialized_projection_splits_per_ipu := self.ipu_config._serialized_projection_splits_per_ipu) is not None:
+            serialized_projection_ipus = [i for i, x in enumerate(serialized_projection_splits_per_ipu) if x]
+            if len(serialized_projection_ipus) > 1:
+                # This is because we are using SerializedLinear. All splits of a SerializedLinear layer must be on the
+                # same IPU. We are using SerializedLinear instead of SplitLinear because we must tie the weights, which
+                # cannot be done when using SplitLinear.
+                raise ValueError(
+                    "`serialized_projection_splits_per_ipu` must only have 1 non-zero element for Whisper."
+                )
+            decoder_embedding_ipu = serialized_projection_ipus[0]
+        self.model.decoder.embed_tokens = poptorch.BeginBlock(
+            self.model.decoder.embed_tokens, "Decoder Embedding", ipu_id=decoder_embedding_ipu
         )
+        logger.info(f"Decoder Embedding  --> IPU {decoder_embedding_ipu}")
 
-        for index, (layer, ipu) in enumerate(zip(self.decoder.block, decoder_layer_ipu)):
-            if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_layers - 1:
+        for index, (layer, ipu) in enumerate(zip(self.model.decoder.layers, decoder_layer_ipu)):
+            if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_hidden_layers - 1:
                 self._hooks.append(recomputation_checkpoint(layer))
-            self.decoder.block[index] = poptorch.BeginBlock(layer, f"Decoder{index}", ipu_id=ipu)
+            self.model.decoder.layers[index] = poptorch.BeginBlock(layer, f"Decoder{index}", ipu_id=ipu)
             logger.info(f"Decoder {index:<2} --> IPU {ipu}")
 
-        self.decoder.final_layer_norm = poptorch.BeginBlock(
-            self.decoder.final_layer_norm, "Decoder Stack Final LayerNorm", ipu_id=ipu
+        self.model.decoder.layer_norm = poptorch.BeginBlock(
+            self.model.decoder.layer_norm, "Decoder Layer Norm", ipu_id=ipu
         )
 
-        logger.info("LM Head Output --> IPU 0")
-        self.lm_head = poptorch.BeginBlock(self.lm_head, "LM Head Output", ipu_id=0)
-        logger.info("-----------------------------------------------------------")
+        logger.info(f"Head       --> IPU {decoder_embedding_ipu}")
+        logger.info("---------------------------------------")
+        self.proj_out = poptorch.BeginBlock(self.proj_out, "Output Projection", ipu_id=decoder_embedding_ipu)
         return self
 
     def deparallelize(self):
-        """
-        Undo the changes to the model done by `parallelize`.
-        You should call this before doing `save_pretrained` so that the `model.state_dict` is
-        fully compatible with `transformers.T5ForConditionalGeneration`.
-        """
-        # T5ForConditionalGeneration has a deparallelize method, so make sure that the PipelineMixin one is used here.
-        PipelineMixin.deparallelize(self)
+        super().deparallelize()
 
-        self.encoder_and_decoder_embeddings_computation(False)
+        self.change_encoder_layer_class(restore=True)
+        self.change_decoder_class(restore=True)
+        self.change_decoder_positional_embedding(restore=True)
+        self.change_attention_class(restore=True)
+        self.change_lm_head(restore=True)
+        self.change_encoder_class(restore=True)
+        self.set_on_device_generation_steps(0)
 
-        self.encoder.__class__ = T5Stack
-        self.decoder.__class__ = T5Stack
+        return self
 
-        self.encoder.embed_tokens = self.encoder.embed_tokens.module
-
-        for block in self.encoder.block:
-            block.__class__ = T5Block
-            block.layer[0].dropout = block.layer[0].dropout.module
-            with torch.no_grad():
-                block.layer[1].DenseReluDense.wo.weight *= block.layer[1].dropout.scale
-            block.layer[1].dropout = block.layer[1].dropout.module
-            if self.config.dense_act_fn == "gelu_new":
-                block.layer[1].DenseReluDense.act = NewGELUActivation()
-        for block in self.decoder.block:
-            block.__class__ = T5Block
-            if self.config.dense_act_fn == "gelu_new":
-                block.layer[2].DenseReluDense.act = NewGELUActivation()
-
-        self.change_lm_head_to_indexed_input_linear(restore=True)
-
-        if isinstance(self.lm_head, SerializedLinear):
-            self.lm_head = self.lm_head.to_model()
-            # TODO: is it needed to check?
-            if self.config.tie_word_embeddings:
-                self.tie_weights()
+    def prepare_inputs_for_generation(
+        self,
+        decoder_input_ids,
+        past_key_values=None,
+        use_cache=None,
+        encoder_outputs=None,
+        attention_mask=None,
+        **kwargs,
+    ):
+        # We don't use `past_key_values` for KV caching, and rely on `use_cache` instead.
+        beam_idx = None
+        if use_cache:
+            decoder_input_ids = decoder_input_ids[:, -1:]
+            beam_idx = kwargs.get("beam_idx", torch.arange(decoder_input_ids.shape[0], dtype=torch.long))
 
-        return self
+        ret = {
+            "past_key_values": None,
+            "decoder_input_ids": decoder_input_ids,
+            "decoder_attention_mask": None,
+            "beam_idx": beam_idx,
+        }
+        if self.cond_encoder_enabled:
+            input_features = kwargs.get("input_features", None)
+            if input_features is None:
+                raise ValueError("Missing `input_features` with `use_cond_encoder=True`.")
+            ret["input_features"] = input_features
+        else:
+            ret["encoder_outputs"] = encoder_outputs
+        return ret
 
+    # TODO: consider making such output subsetting a decorator
     def forward(
         self,
-        input_ids: Optional[torch.LongTensor] = None,
-        attention_mask: Optional[torch.FloatTensor] = None,
+        input_features: Optional[torch.FloatTensor] = None,
+        attention_mask: Optional[torch.LongTensor] = None,
         decoder_input_ids: Optional[torch.LongTensor] = None,
-        decoder_attention_mask: Optional[torch.BoolTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        decoder_head_mask: Optional[torch.FloatTensor] = None,
+        decoder_attention_mask: Optional[torch.LongTensor] = None,
+        head_mask: Optional[torch.Tensor] = None,
+        decoder_head_mask: Optional[torch.Tensor] = None,
         cross_attn_head_mask: Optional[torch.Tensor] = None,
-        encoder_outputs: Optional[Tuple[Tuple[torch.Tensor]]] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
-        inputs_embeds: Optional[torch.FloatTensor] = None,
-        decoder_inputs_embeds: Optional[torch.FloatTensor] = None,
+        encoder_outputs: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
+        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
+        decoder_inputs_embeds: Optional[Tuple[torch.FloatTensor]] = None,
         labels: Optional[torch.LongTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[torch.FloatTensor], Seq2SeqLMOutput]:
-        use_cache = use_cache if use_cache is not None else self.config.use_cache
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        if self.is_encoder_and_decoder_embeddings_computation_shared:
-            inputs_embeds, decoder_inputs_embeds = self.shared(
-                input_ids=input_ids,
-                decoder_input_ids=decoder_input_ids,
-            )
-            if inputs_embeds is not None:
-                input_ids = None
-            if decoder_inputs_embeds is not None:
-                decoder_input_ids = None
-
-        # FutureWarning: head_mask was separated into two input args - head_mask, decoder_head_mask
-        if head_mask is not None and decoder_head_mask is None:
-            if self.config.num_layers == self.config.num_decoder_layers:
-                warnings.warn(__HEAD_MASK_WARNING_MSG, FutureWarning)
-                decoder_head_mask = head_mask
-
-        # Encode if needed (training, first prediction pass)
-        if encoder_outputs is None:
-            # Convert encoder inputs in embeddings if needed
-            encoder_outputs = self.encoder(
-                input_ids=input_ids,
-                attention_mask=attention_mask,
-                inputs_embeds=inputs_embeds,
-                head_mask=head_mask,
-                output_attentions=output_attentions,
-                output_hidden_states=output_hidden_states,
-                return_dict=return_dict,
-            )
-        elif return_dict and not isinstance(encoder_outputs, BaseModelOutput):
-            encoder_outputs = BaseModelOutput(
-                last_hidden_state=encoder_outputs[0],
-                hidden_states=encoder_outputs[1] if len(encoder_outputs) > 1 else None,
-                attentions=encoder_outputs[2] if len(encoder_outputs) > 2 else None,
-            )
-
-        hidden_states = encoder_outputs[0]
+    ) -> Union[Tuple[torch.Tensor], Seq2SeqLMOutput]:
+        # Duplicate this portion of upstream logic so we can intercept the call to `shift_tokens_right`.
+        if labels is not None:
+            if decoder_input_ids is None and decoder_inputs_embeds is None:
+                decoder_input_ids = shift_tokens_right(
+                    labels, self.config.pad_token_id, self.config.decoder_start_token_id
+                )
 
-        if labels is not None and decoder_input_ids is None and decoder_inputs_embeds is None:
-            # get decoder inputs from shifting lm labels to the right
-            decoder_input_ids = self._shift_right(labels)
-
-        # Decode
-        decoder_outputs = self.decoder(
-            input_ids=decoder_input_ids,
-            attention_mask=decoder_attention_mask,
-            inputs_embeds=decoder_inputs_embeds,
-            past_key_values=past_key_values,
-            encoder_hidden_states=hidden_states,
-            encoder_attention_mask=attention_mask,
-            head_mask=decoder_head_mask,
+        output = super().forward(
+            input_features=input_features,
+            attention_mask=attention_mask,
+            decoder_input_ids=decoder_input_ids,
+            decoder_attention_mask=decoder_attention_mask,
+            head_mask=head_mask,
+            decoder_head_mask=decoder_head_mask,
             cross_attn_head_mask=cross_attn_head_mask,
+            encoder_outputs=encoder_outputs,
+            past_key_values=past_key_values,
+            decoder_inputs_embeds=decoder_inputs_embeds,
+            labels=labels,
             use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
+            return_dict=True,
         )
 
-        sequence_output = decoder_outputs[0]
-
-        # Set device for model parallelism
-        if self.model_parallel:
-            self.lm_head = self.lm_head.to(self.encoder.first_device)
-            sequence_output = sequence_output.to(self.lm_head.weight.device)
-
-        if self.config.tie_word_embeddings:
-            # Rescale output before projecting on vocab
-            # See https://github.com/tensorflow/mesh/blob/fa19d69eafc9a482aff0b59ddd96b025c0cb207d/mesh_tensorflow/transformer/transformer.py#L586
-            sequence_output = sequence_output * (self.model_dim**-0.5)
-
-        lm_scale_modifier = getattr(self, "lm_scale_modifier", None)
-        if lm_scale_modifier is not None:
-            sequence_output = sequence_output * lm_scale_modifier
-
-        lm_logits = self.lm_head(sequence_output)
-
-        loss = None
-        if labels is not None:
-            loss_fct = nn.CrossEntropyLoss(ignore_index=-100)
-            loss = loss_fct(lm_logits.view(-1, lm_logits.size(-1)), labels.view(-1))
-        # TODO(thom): Add z_loss https://github.com/tensorflow/mesh/blob/fa19d69eafc9a482aff0b59ddd96b025c0cb207d/mesh_tensorflow/layers.py#L666
-
-        # Only returning the loss to make the communication between the host and the device faster.
-        if not return_dict:
-            output = (lm_logits,) + decoder_outputs[1:] + encoder_outputs
-            return (loss,) if labels is not None else output
-
-        if loss is not None:
-            return Seq2SeqLMOutput(
-                loss=loss,
-            )
-
+        # Minimize IO and only return loss when training.
         return Seq2SeqLMOutput(
-            loss=loss,
-            logits=lm_logits,
-            past_key_values=decoder_outputs.past_key_values,
-            decoder_hidden_states=decoder_outputs.hidden_states,
-            decoder_attentions=decoder_outputs.attentions,
-            cross_attentions=decoder_outputs.cross_attentions,
-            encoder_last_hidden_state=encoder_outputs.last_hidden_state,
-            encoder_hidden_states=encoder_outputs.hidden_states,
-            encoder_attentions=encoder_outputs.attentions,
-        )
-
-
-@register(T5EncoderModel)
-class PipelinedT5EncoderModel(T5EncoderModel, PipelineMixin):
-    def parallelize(self):
-        """
-        Transform the model to run in an IPU pipeline.
-        - Adds pipeline stages to the model
-        - Adds recomputation checkpoints
-
-        Recommended usage:
-        ```
-        model = PipelinedT5EncoderModel(config).parallelize().half()
-        ```
-        """
-        PipelineMixin.parallelize(self)
-
-        logger.info("-------------------- Device Allocation --------------------")
-        logger.info("Embedding  --> IPU 0")
-
-        self.shared = poptorch.BeginBlock(self.shared, "Embedding", ipu_id=0)
-
-        # Use a custom T5Stack implementation because sharing the position bias causes OOM error
-        self.encoder.__class__ = CustomT5Stack
-
-        # Upcast input embeddings so that the residuals remain in FP32. This
-        # cast is reversed where necessary by the T5LayerNorm layers in:
-        # - first layer of T5LayerSelfAttention
-        # - first layer of T5LayerFF
-        # - final_layer_norm
-        # Which, conveniently, are all the places that this needs to happen.
-        # Therefore, so we just need to upcast immediately before the residual
-        # adds in T5LayerSelfAttention and T5LayerFF. This is handled in the
-        # for loop below.
-        self.encoder.embed_tokens = UpCastWrapper(self.encoder.embed_tokens)
-
-        # Use a custom T5Block implementation that removes a dynamic if blocks that can't be statically traced
-        for block in self.encoder.block:
-            block.__class__ = CustomT5Block
-            # Dropout happens immediately before the residual add. Inserting a
-            # cast in T5LayerSelfAttention and T5LayerFF keeps the residual
-            # structure in FP32
-            block.layer[0].dropout = UpCastWrapper(block.layer[0].dropout)
-            # Scale down the weights for the T5LayerFF down-projection and
-            # then scale its output back up again after it is cast to FP32
-            scale = 8.0
-            with torch.no_grad():
-                block.layer[1].DenseReluDense.wo.weight /= scale
-            block.layer[1].dropout = UpCastWrapper(block.layer[1].dropout, scale)
-            # Prevent overflow in NewGELUActivation
-            if self.config.dense_act_fn == "gelu_new":
-                # TODO: Work-around bug with torch.nn.GELU(approximate="tanh"). Replace
-                # this with block.layer[1].DenseReluDense.act = torch.nn.GELU(approximate="tanh")
-                # when bug is fixed
-                block.layer[1].DenseReluDense.act = CustomGELU()
-
-        num_encoder_layers = len(self.encoder.block)
-        number_of_layers = num_encoder_layers
-        encoder_layer_ipu = get_layer_ipu(self.ipu_config, number_of_layers)
-
-        for index, (layer, ipu) in enumerate(zip(self.encoder.block, encoder_layer_ipu)):
-            if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_layers - 1:
-                self._hooks.append(recomputation_checkpoint(layer))
-            self.encoder.block[index] = poptorch.BeginBlock(layer, f"Encoder{index}", ipu_id=ipu)
-            logger.info(f"Encoder {index:<2} --> IPU {ipu}")
-
-        self.encoder.final_layer_norm = poptorch.BeginBlock(
-            self.encoder.final_layer_norm, "Encoder Stack Final LayerNorm", ipu_id=ipu
+            loss=output.loss,
+            logits=None if self.training else output.logits,
+            encoder_last_hidden_state=None if self.training else output.encoder_last_hidden_state,  # for tests to pass
+            past_key_values=None if self.training else output.past_key_values,  # for tests to pass
         )
-
-        return self
-
-    def deparallelize(self):
-        """
-        Undo the changes to the model done by `parallelize`.
-        You should call this before doing `save_pretrained` so that the `model.state_dict` is
-        fully compatible with `transformers.T5ForConditionalGeneration`.
-        """
-        # T5ForConditionalGeneration has a deparallelize method, so make sure that the PipelineMixin one is used here.
-        PipelineMixin.deparallelize(self)
-
-        self.encoder.__class__ = T5Stack
-        self.encoder.embed_tokens = self.encoder.embed_tokens.module
-
-        for block in self.encoder.block:
-            block.__class__ = T5Block
-            block.layer[0].dropout = block.layer[0].dropout.module
-            with torch.no_grad():
-                block.layer[1].DenseReluDense.wo.weight *= block.layer[1].dropout.scale
-            block.layer[1].dropout = block.layer[1].dropout.module
-            if self.config.dense_act_fn == "gelu_new":
-                block.layer[1].DenseReluDense.act = NewGELUActivation()
-
-        return self
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/vit/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/vit/modeling_vit.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/vit/modeling_vit.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/wav2vec2/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/whisper/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/feature_extraction_whisper.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/whisper/feature_extraction_whisper.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/processing_whisper.py` & `optimum-graphcore-0.7.1/optimum/graphcore/models/whisper/processing_whisper.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/pipelines/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/pipelines/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,42 +213,43 @@
 
 def get_poplar_executor(
     task: str,
     model: PreTrainedModel,
     ipu_config: Union[IPUConfig, str, dict] = None,
     fp16: bool = True,
     for_generation: bool = False,
-    **parallelize_kwargs,
 ) -> PreTrainedModel:
     ipu_config_arg = ipu_config
 
     if isinstance(ipu_config, str):
         ipu_config = IPUConfig.from_pretrained(ipu_config)
     elif isinstance(ipu_config, dict):
         ipu_config = IPUConfig.from_dict(ipu_config)
     elif not isinstance(ipu_config, IPUConfig):
         raise ValueError("ipu_config must be an IPUConfig, string, or a dictionary.")
 
     # So that IPUConfig returns inference versions of any parameters
     # that are different in training and inference
     ipu_config.eval()
 
+    parallelize_kwargs = ipu_config.inference_parallelize_kwargs
+
     ipu_config.inference_device_iterations = 1
     if not parallelize_kwargs.get("use_cond_encoder", False):
         ipu_config.inference_replication_factor = 1
     if not fp16:
         ipu_config.enable_half_partials = False
     try:
         model = to_pipelined(model, ipu_config, force=False)
         if model.config.is_encoder_decoder and isinstance(model, IPUGenerationMixin):
             if "use_cache" not in parallelize_kwargs and model.__class__ in MODELS_SUPPORTING_KV_CACHE:
                 parallelize_kwargs["use_cache"] = True
             model.parallelize(for_generation=for_generation, **parallelize_kwargs)
         else:
-            model.parallelize()
+            model.parallelize(**parallelize_kwargs)
     except Exception as error:
         new_message = (
             "The model and ipu_config seem to be incompatible,"
             " please try a different IPU config or customize it for the model."
             f" The config provided is '{ipu_config_arg}'\n"
             f"{error}"
         )
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/pipelines/automatic_speech_recognition.py` & `optimum-graphcore-0.7.1/optimum/graphcore/pipelines/automatic_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/pipelines/fill_mask.py` & `optimum-graphcore-0.7.1/optimum/graphcore/pipelines/fill_mask.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/pipelines/text2text_generation.py` & `optimum-graphcore-0.7.1/optimum/graphcore/pipelines/text2text_generation.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/pipelines/token_classification.py` & `optimum-graphcore-0.7.1/optimum/graphcore/pipelines/token_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/pipelines/zero_shot_classification.py` & `optimum-graphcore-0.7.1/optimum/graphcore/pipelines/zero_shot_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/trainer.py` & `optimum-graphcore-0.7.1/optimum/graphcore/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
             if self.args.do_eval:
                 data_collator_wrapper = pad_on_batch_axis(
                     self.args.per_device_eval_batch_size * self.ipu_config.batch_size_factor(for_inference=True),
                 )
                 self.eval_data_collator = data_collator_wrapper(self.eval_data_collator)
 
         self.model = to_pipelined(model, self.ipu_config, force=force_to_pipelined)
-        self.model.parallelize()
+        self.model.parallelize(**self.ipu_config.parallelize_kwargs)
 
         self.original_model = model
 
         if not self.args.fp32:
             self.model = self.model.half()
 
         self.training_model = None
@@ -383,15 +383,22 @@
 
         # If compile-only then compile and exit
         if args.compile_only:
             logger.info("Called with compile_only=True. Compiling models then exiting.")
             if args.do_train:
                 train_dl = self.get_train_dataloader()
                 model = self.wrap_model(self.model)
-                self.compile_model(model, next(iter(train_dl)), log=True)
+                try:
+                    model_inputs = next(iter(train_dl))
+                except StopIteration:
+                    raise ValueError(
+                        "Couldn't get first sample from dataloader, please check for warnings "
+                        "during dataloader construction."
+                    )
+                self.compile_model(model, model_inputs, log=True)
             if args.do_eval:
                 # Same thing with _wrap_and_compile_for_evaluation
                 eval_dl = self.get_eval_dataloader()
                 model = self._wrap_and_compile_model_for_evaluation(eval_dl, False)
             logger.info("Exiting after compiling models with compile_only=True")
             sys.exit(0)
 
@@ -609,14 +616,44 @@
                 model_input_name=model_input_name,
                 generator=generator,
             )
 
         else:
             return RandomSampler(self.train_dataset)
 
+    def _check_dataset_can_fill_batch(self, dataset: torch.utils.data.Dataset, for_inference: bool = False) -> None:
+        replication_factor = (
+            self.ipu_config.inference_replication_factor if for_inference else self.ipu_config.replication_factor
+        )
+        gradient_accumulation_steps = 1 if for_inference else self.ipu_config.gradient_accumulation_steps
+        device_iterations = (
+            self.ipu_config.inference_device_iterations if for_inference else self.ipu_config.device_iterations
+        )
+        micro_batch_size = (
+            self.args.per_device_eval_batch_size if for_inference else self.args.per_device_train_batch_size
+        )
+        global_batch_size = micro_batch_size * replication_factor * gradient_accumulation_steps * device_iterations
+
+        try:
+            len(dataset)
+        except Exception:
+            # If the length of the dataset cannot be determined skip the checks
+            return
+        if len(dataset) < global_batch_size:
+            mode_str = "inference_" if for_inference else ""
+            logger.warning(
+                f"The provided dataset is of length {len(dataset)}, but the total dataset batch size is {global_batch_size}. "
+                f"This batch size is calculated as:\n"
+                f"  per_device_{'eval' if for_inference else 'train'}_batch_size={micro_batch_size}\n"
+                f"* {mode_str}{replication_factor=}\n"
+                f"* {mode_str}{gradient_accumulation_steps=}\n"
+                f"* {mode_str}{device_iterations=}\n"
+                "Please disregard this warning if you believe the dataset is reporting an incorrect length, such as 1."
+            )
+
     def get_train_dataloader(self) -> poptorch.DataLoader:
         """
         Returns the training `poptorch.DataLoader`.
 
         Will not use a sampler if `train_dataset` does not implement `__len__` and will use a random sampler (adapted to distributed
         training if necessary) otherwise.
 
@@ -654,14 +691,16 @@
         combined_batch_size = self.args.per_device_train_batch_size * self.ipu_config.batch_size_factor()
         rebatched_worker_size = (
             2 * (combined_batch_size // self.args.dataloader_num_workers)
             if self.args.dataloader_num_workers
             else combined_batch_size
         )
 
+        self._check_dataset_can_fill_batch(train_dataset, for_inference=False)
+
         return poptorch.DataLoader(
             self.opts,
             train_dataset,
             batch_size=self.args.per_device_train_batch_size,
             sampler=train_sampler,
             collate_fn=self.data_collator,
             num_workers=self.args.dataloader_num_workers,
@@ -709,14 +748,16 @@
                 num_workers=self.args.dataloader_num_workers,
                 pin_memory=self.args.dataloader_pin_memory,
                 **poptorch_specific_kwargs,
             )
 
         eval_sampler = self._get_eval_sampler(eval_dataset)
 
+        self._check_dataset_can_fill_batch(eval_dataset, for_inference=True)
+
         return poptorch.DataLoader(
             self.eval_opts,
             eval_dataset,
             sampler=eval_sampler,
             batch_size=self.args.per_device_eval_batch_size,
             collate_fn=data_collator,
             drop_last=self.args.dataloader_drop_last,
@@ -757,14 +798,16 @@
                 num_workers=self.args.dataloader_num_workers,
                 pin_memory=self.args.dataloader_pin_memory,
                 **poptorch_specific_kwargs,
             )
 
         test_sampler = self._get_eval_sampler(test_dataset)
 
+        self._check_dataset_can_fill_batch(test_dataset, for_inference=True)
+
         # We use the same batch_size as for eval.
         return poptorch.DataLoader(
             self.eval_opts,
             test_dataset,
             sampler=test_sampler,
             batch_size=self.args.per_device_eval_batch_size,
             collate_fn=data_collator,
@@ -904,25 +947,25 @@
         wrapped = None
         if isinstance(model, PoplarExecutor):
             wrapped = model
         elif training:
             if self.training_model is None:
                 model.deparallelize()
                 model.ipu_config.train()
-                model.parallelize()
+                model.parallelize(**model.ipu_config.parallelize_kwargs)
                 self.create_optimizer()
                 self.training_model = poptorch.trainingModel(
                     model.train(), options=self.opts, optimizer=self.optimizer
                 )
             wrapped = self.training_model
         else:
             if self.inference_model is None:
                 model.deparallelize()
                 model.ipu_config.eval()
-                model.parallelize()
+                model.parallelize(**model.ipu_config.inference_parallelize_kwargs)
                 self.inference_model = poptorch.inferenceModel(model.eval(), options=self.eval_opts)
             wrapped = self.inference_model
 
         # Attaching to device when the model that is being access was already compiled but detached from previous loop.
         if wrapped.isCompiled() and not wrapped.isAttachedToDevice():
             wrapped.attachToDevice()
         return wrapped
@@ -1066,15 +1109,22 @@
         # TODO: handle optimizer and scheduler creation
         # if delay_optimizer_creation:
         #     self.create_optimizer_and_scheduler(num_training_steps=max_steps)
 
         # Check if saved optimizer or scheduler states exist
         self._load_optimizer_and_scheduler(resume_from_checkpoint)
 
-        self.compile_model(self.training_model, next(iter(train_dataloader)), log=True)
+        try:
+            model_inputs = next(iter(train_dataloader))
+        except StopIteration:
+            raise ValueError(
+                "Couldn't get first sample from dataloader, please check for warnings "
+                "during dataloader construction."
+            )
+        self.compile_model(self.training_model, model_inputs, log=True)
 
         # Train!
         num_examples = (
             self.num_examples(train_dataloader)
             if has_length(train_dataloader)
             else total_train_batch_size * args.max_steps
         )
@@ -1315,15 +1365,15 @@
                 f"Could not locate the best model at {best_model_path}. If you are running a distributed training "
                 "on multiple nodes, you should activate `--save_on_each_node`."
             )
 
     def _load_state_dict_in_model(self, state_dict):
         self.model.deparallelize()
         load_result = self.model.load_state_dict(state_dict, strict=False)
-        self.model.parallelize()
+        self.model.parallelize(**self.model.ipu_config._parallelize_kwargs)
         if not self.args.fp32:
             self.model.half()
 
         if len(load_result.missing_keys) != 0:
             if self.model._keys_to_ignore_on_save is not None and set(load_result.missing_keys) != set(
                 self.model._keys_to_ignore_on_save
             ):
@@ -1632,15 +1682,15 @@
             if state_dict is None:
                 state_dict = self.model.state_dict()
             torch.save(state_dict, os.path.join(output_dir, WEIGHTS_NAME))
         else:
             rng_state = torch.random.get_rng_state()
             self.model.deparallelize()
             self.model.save_pretrained(output_dir, state_dict=state_dict)
-            self.model.parallelize()
+            self.model.parallelize(**self.model.ipu_config.parallelize_kwargs)
             torch.random.set_rng_state(rng_state)
 
         if self.tokenizer is not None:
             self.tokenizer.save_pretrained(output_dir)
 
         self.ipu_config.save_pretrained(output_dir)
 
@@ -1845,15 +1895,22 @@
 
         self._memory_tracker.stop_and_update_metrics(output.metrics)
 
         return PredictionOutput(predictions=output.predictions, label_ids=output.label_ids, metrics=output.metrics)
 
     def _wrap_and_compile_model_for_evaluation(self, dataloader, prediction_loss_only):
         model = self.wrap_model(self.model, training=False)
-        self.compile_model(model, next(iter(dataloader)), log=True)
+        try:
+            model_inputs = next(iter(dataloader))
+        except StopIteration:
+            raise ValueError(
+                "Couldn't get first sample from dataloader, please check for warnings "
+                "during dataloader construction."
+            )
+        self.compile_model(model, model_inputs, log=True)
         return model
 
     def evaluation_loop(
         self,
         dataloader: poptorch.DataLoader,
         description: str,
         prediction_loss_only: Optional[bool] = None,
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/trainer_pt_utils.py` & `optimum-graphcore-0.7.1/optimum/graphcore/trainer_pt_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/trainer_seq2seq.py` & `optimum-graphcore-0.7.1/optimum/graphcore/trainer_seq2seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,25 +127,25 @@
         # Unwrap the model, including parameter and buffer annotations and the
         # model as a whole. This is needed to avoid issues with persistent buffers
         # when compiling an inference model for generation
         unwrapModelIfNecessary(self.model)
 
         # reparallelize for generation
         self.model.deparallelize().ipu_config.eval()
-        self.model.parallelize(for_generation=True)
+        self.model.parallelize(for_generation=True, **self.model.ipu_config.inference_parallelize_kwargs)
 
         # let IPUGenerationMixin::_call_generate handle compilation of the model
         # note though that self.model.poptorch_decoder and self.model.poptorch_encoder
         # (attribute added by IPUGenerationMixin::_call_generate)
         # are the actual models attached to the device
         return self.model
 
     def _rewrap_model_for_training(self):
         self.model.deparallelize().ipu_config.train()
-        self.model.parallelize()
+        self.model.parallelize(**self.model.ipu_config.parallelize_kwargs)
         # Restores the PoptorchParameter and PoptorchBuffer annotations in the model
         rewrapModelIfNecessary(self.model)
 
     def evaluate(
         self,
         eval_dataset: Optional[Dataset] = None,
         ignore_keys: Optional[List[str]] = None,
```

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/trainer_utils.py` & `optimum-graphcore-0.7.1/optimum/graphcore/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/training_args.py` & `optimum-graphcore-0.7.1/optimum/graphcore/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/training_args_seq2seq.py` & `optimum-graphcore-0.7.1/optimum/graphcore/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/utils/__init__.py` & `optimum-graphcore-0.7.1/optimum/graphcore/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/optimum/graphcore/version.py` & `optimum-graphcore-0.7.1/optimum/graphcore/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
```

### Comparing `optimum-graphcore-0.7.0/optimum_graphcore.egg-info/PKG-INFO` & `optimum-graphcore-0.7.1/optimum_graphcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-graphcore
-Version: 0.7.0
+Version: 0.7.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://huggingface.co/hardware
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,training,ipu
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `optimum-graphcore-0.7.0/pyproject.toml` & `optimum-graphcore-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/setup.py` & `optimum-graphcore-0.7.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 
 INSTALL_REQUIRES = [
     "transformers==4.29.2",
     "optimum==1.6.1",
     "diffusers[torch]==0.12.1",
+    "cppimport==22.8.2",
     "datasets",
     "tokenizers",
     "typeguard",
     "sentencepiece",
     "scipy",
     "pillow",
 ]
@@ -57,14 +58,15 @@
         "pytest-xdist",
         "librosa",
         "soundfile",
     ],
     "quality": QUALITY_REQUIRES,
 }
 
+
 setup(
     name="optimum-graphcore",
     version=__version__,
     description="Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to "
     "integrate third-party libraries from Hardware Partners and interface with their specific "
     "functionality.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
@@ -86,8 +88,9 @@
     author_email="hardware@huggingface.co",
     license="Apache",
     packages=find_namespace_packages(include=["optimum*"]),
     install_requires=INSTALL_REQUIRES,
     extras_require=EXTRA_REQUIRE,
     include_package_data=True,
     zip_safe=False,
+    package_data={"": ["*.cpp", "*.hpp"]}
 )
```

### Comparing `optimum-graphcore-0.7.0/tests/test_examples.py` & `optimum-graphcore-0.7.1/tests/test_examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,33 +36,34 @@
     MODEL_FOR_QUESTION_ANSWERING_MAPPING,
     MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING,
     MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING,
     MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING,
 )
 from transformers.testing_utils import slow
 
+from optimum.graphcore import IPUConfig
 from optimum.graphcore.modeling_utils import _PRETRAINED_TO_PIPELINED_REGISTRY
 
-from .utils import MODELS_TO_TEST_MAPPING
+from .utils import MODELS_TO_TEST_MAPPING, high_memory_usage
 
 
 def _get_supported_models_for_script(
     models_to_test: Dict[str, Tuple[str]], task_mapping: Dict[str, str], task: str = "default"
 ) -> List[Tuple[str]]:
     """
     Filters models that can perform the task from models_to_test.
 
     Args:
-        models_to_test: mapping between a model type and a tuple (model_name_or_path, ipu_config_name).
+        models_to_test: mapping between a model type and a tuple (model_name_or_path, ipu_config).
         task_mapping: mapping bewteen a model config and a model class.
         task: the task to get the model names for.
 
     Returns:
         A list of models that are supported for the task.
-        Each element of the list follows the same format: (model_type, (model_name_or_path, ipu_config_name)).
+        Each element of the list follows the same format: (model_type, (model_name_or_path, ipu_config)).
     """
 
     def is_valid_model_type(model_type: str) -> bool:
         in_task_mapping = CONFIG_MAPPING[model_type] in task_mapping
         if in_task_mapping:
             return task_mapping[CONFIG_MAPPING[model_type]] in _PRETRAINED_TO_PIPELINED_REGISTRY
         return False
@@ -78,18 +79,18 @@
 
 _SCRIPT_TO_MODEL_MAPPING = {
     "run_clm": _get_supported_models_for_script(MODELS_TO_TEST_MAPPING, MODEL_FOR_CAUSAL_LM_MAPPING),
     "run_mlm": _get_supported_models_for_script(MODELS_TO_TEST_MAPPING, MODEL_FOR_MASKED_LM_MAPPING),
     "run_swag": _get_supported_models_for_script(MODELS_TO_TEST_MAPPING, MODEL_FOR_MULTIPLE_CHOICE_MAPPING),
     "run_qa": _get_supported_models_for_script(MODELS_TO_TEST_MAPPING, MODEL_FOR_QUESTION_ANSWERING_MAPPING),
     "run_summarization": _get_supported_models_for_script(
-        MODELS_TO_TEST_MAPPING, MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING
+        MODELS_TO_TEST_MAPPING, MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING, task="summarization"
     ),
     "run_translation": _get_supported_models_for_script(
-        MODELS_TO_TEST_MAPPING, MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING
+        MODELS_TO_TEST_MAPPING, MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING, task="translation"
     ),
     "run_glue": _get_supported_models_for_script(MODELS_TO_TEST_MAPPING, MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING),
     "run_ner": _get_supported_models_for_script(MODELS_TO_TEST_MAPPING, MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING),
     "run_image_classification": _get_supported_models_for_script(
         MODELS_TO_TEST_MAPPING, MODEL_FOR_IMAGE_CLASSIFICATION_MAPPING
     ),
     "run_audio_classification": _get_supported_models_for_script(
@@ -114,27 +115,32 @@
     def __new__(cls, name, bases, attrs, example_name=None):
         models_to_test = []
         if example_name is not None:
             models_to_test = _SCRIPT_TO_MODEL_MAPPING.get(example_name)
             if models_to_test is None:
                 raise AttributeError(f"could not create class because no model was found for example {example_name}")
         for model_type, names in models_to_test:
-            model_name, ipu_config_name = names
-            attrs[f"test_{example_name}_{model_type}"] = cls._create_test(model_name, ipu_config_name)
+            model_name, ipu_config, example_config = names
+            test_name = f"test_{example_name}_{model_type}"
+            attrs[test_name] = cls._create_test(model_name, ipu_config, example_config)
+            if name == "SummarizationExampleTester" and model_name == "google/mt5-small":
+                attrs[test_name] = high_memory_usage(attrs[test_name])
         attrs["EXAMPLE_NAME"] = example_name
         return super().__new__(cls, name, bases, attrs)
 
     @classmethod
-    def _create_test(cls, model_name: str, ipu_config_name: str) -> Callable[[], None]:
+    def _create_test(
+        cls, model_name: str, ipu_config: Union[str, IPUConfig], example_config: Dict
+    ) -> Callable[[], None]:
         """
-        Creates a test function that runs an example for a specific (model_name, ipu_config_name) pair.
+        Creates a test function that runs an example for a specific (model_name, ipu_config) pair.
 
         Args:
             model_name: the model_name_or_path.
-            ipu_config_name: the ipu config name.
+            ipu_config: IPUConfig instance or the ipu config name.
 
         Returns:
             The test function that runs the example.
         """
 
         @slow
         def test(self):
@@ -145,33 +151,63 @@
             if len(example_script) == 0:
                 raise RuntimeError(f"Could not find {self.EXAMPLE_NAME}.py in examples located in {self.EXAMPLE_DIR}")
             elif len(example_script) > 1:
                 raise RuntimeError(f"Found more than {self.EXAMPLE_NAME}.py in examples located in {self.EXAMPLE_DIR}")
             else:
                 example_script = example_script[0]
 
-            self._install_requirements(example_script.parent / "requirements.txt")
+            command_line_kwargs = {
+                "task": self.TASK_NAME,
+                "dataset_config_name": self.DATASET_CONFIG_NAME,
+                "do_eval": self.EVAL_IS_SUPPORTED,
+                "lr": self.LEARNING_RATE,
+                "train_batch_size": self.TRAIN_BATCH_SIZE,
+                "eval_batch_size": self.EVAL_BATCH_SIZE,
+                "num_epochs": self.NUM_EPOCHS,
+                "max_steps": self.MAX_STEPS,
+                "inference_device_iterations": self.INFERENCE_DEVICE_ITERATIONS,
+                "gradient_accumulation_steps": self.GRADIENT_ACCUMULATION_STEPS,
+                "extra_command_line_arguments": self.EXTRA_COMMAND_LINE_ARGUMENTS,
+            }
+
+            def to_dict(input_list: list):
+                """
+                helper function to convert EXTRA_COMMAND_LINE_ARGUMENTS list
+                to a map
+                """
+                output = {}
+                for param_value in input_list:
+                    split_param_value = param_value.split(" ", 1)
+                    if len(split_param_value) > 1:
+                        param, value = split_param_value
+                        output[param] = value
+                    else:
+                        output[param_value] = ""
+                return output
 
-            with TemporaryDirectory(dir=Path(self.EXAMPLE_DIR)) as tmp_dir:
+            for config, value in example_config.items():
+                if config in command_line_kwargs:
+                    if config == "extra_command_line_arguments":
+                        updated_defaults = to_dict(command_line_kwargs[config])
+                        override = to_dict(example_config[config])
+                        updated_defaults.update(override)
+                        command_line_kwargs[config] = [
+                            param + " " + value for param, value in updated_defaults.items()
+                        ]
+                    else:
+                        command_line_kwargs[config] = value
+                else:
+                    raise KeyError(f"{example_config=} can only override the following keys: {command_line_kwargs=}")
+
+            with TemporaryDirectory(dir=Path(self.EXAMPLE_DIR).resolve()) as tmp_dir:
+                self._create_venv(tmp_dir)
+                self._install_requirements(example_script.parent / "requirements.txt")
                 os.environ["HF_HOME"] = os.path.join(tmp_dir, "hf_home")
                 cmd_line = self._create_command_line(
-                    example_script,
-                    model_name,
-                    ipu_config_name,
-                    tmp_dir,
-                    task=self.TASK_NAME,
-                    dataset_config_name=self.DATASET_CONFIG_NAME,
-                    do_eval=self.EVAL_IS_SUPPORTED,
-                    lr=self.LEARNING_RATE,
-                    train_batch_size=self.TRAIN_BATCH_SIZE,
-                    eval_batch_size=self.EVAL_BATCH_SIZE,
-                    num_epochs=self.NUM_EPOCHS,
-                    inference_device_iterations=self.INFERENCE_DEVICE_ITERATIONS,
-                    gradient_accumulation_steps=self.GRADIENT_ACCUMULATION_STEPS,
-                    extra_command_line_arguments=self.EXTRA_COMMAND_LINE_ARGUMENTS,
+                    example_script, model_name, ipu_config, tmp_dir, **command_line_kwargs
                 )
                 print()
                 print("#### Running command line... ####")
                 joined_cmd_line = " ".join(cmd_line)
                 print(joined_cmd_line)
                 print()
                 p = subprocess.run(joined_cmd_line, shell=True)
@@ -221,41 +257,37 @@
     EVAL_IS_SUPPORTED = True
     EVAL_SCORE_THRESHOLD = 0.75
     EVAL_SCORE_THRESHOLD_OVERRIDES = None
     EVAL_SCORE_GREATER_IS_BETTER = True
     SCORE_NAME = "eval_accuracy"
     DATASET_PARAMETER_NAME = "dataset_name"
     NUM_EPOCHS = 1
+    MAX_STEPS = -1
     LEARNING_RATE = 1e-4
     TRAIN_BATCH_SIZE = 2
     EVAL_BATCH_SIZE = 2
     INFERENCE_DEVICE_ITERATIONS = 4
     GRADIENT_ACCUMULATION_STEPS = 64
     EXTRA_COMMAND_LINE_ARGUMENTS = None
     N_IPU = 8
 
-    def setUp(self):
-        self._create_venv()
-
-    def tearDown(self):
-        self._remove_venv()
-
     def _create_command_line(
         self,
         script: str,
         model_name: str,
-        ipu_config_name: str,
+        ipu_config: Union[str, IPUConfig],
         output_dir: str,
         task: Optional[str] = None,
         dataset_config_name: Optional[str] = None,
         do_eval: bool = True,
         lr: float = 1e-4,
         train_batch_size: int = 2,
         eval_batch_size: int = 2,
         num_epochs: int = 2,
+        max_steps: int = -1,
         inference_device_iterations: int = 4,
         gradient_accumulation_steps: int = 64,
         extra_command_line_arguments: Optional[List[str]] = None,
     ) -> List[str]:
         do_eval_option = "--do_eval" if do_eval else " "
         task_option = f"--{self.DATASET_PARAMETER_NAME} {task}" if task else " "
         ipu_config_overrides = ",".join(
@@ -263,66 +295,66 @@
                 "executable_cache_dir=disabled",
                 "device_iterations=1",
                 f"inference_device_iterations={inference_device_iterations}",
                 f"gradient_accumulation_steps={gradient_accumulation_steps}",
             ]
         )
 
+        # if the input is an IPUConfig instance, serialize it locally
+        # so that the subprocess can load it
+        if isinstance(ipu_config, IPUConfig):
+            local_config_path = Path(output_dir) / "ipu_config"
+            ipu_config.save_pretrained(local_config_path)
+            ipu_config = local_config_path
+
         cmd_line = [
-            f"{self.VENV_DIR.name}/bin/python" if self.venv_was_created else "python",
+            f"{self.venv_dir}/bin/python" if self.venv_was_created else "python",
             f"{script}",
             f"--model_name_or_path {model_name}",
-            f"--ipu_config_name {ipu_config_name}",
+            f"--ipu_config_name {ipu_config}",
             f"{task_option}",
             "--do_train",
             f"{do_eval_option}",
             f"--output_dir {output_dir}",
             "--overwrite_output_dir true",
             f"--learning_rate {lr}",
             f"--per_device_train_batch_size {train_batch_size}",
             f"--per_device_eval_batch_size {eval_batch_size}",
             "--save_strategy epoch",
             f"--ipu_config_overrides {ipu_config_overrides}",
-            f" --num_train_epochs {num_epochs}",
+            f"--num_train_epochs {num_epochs}",
+            f"--max_steps {max_steps}",
             "--dataloader_num_workers 16",
             "--pad_on_batch_axis",
             "--save_steps -1",
             "--save_total_limit 1",
             "--report_to none",
             f"--n_ipu {self.N_IPU}",
         ]
         if dataset_config_name is not None:
             cmd_line.append(f"--dataset_config_name {dataset_config_name}")
 
         if extra_command_line_arguments is not None:
             cmd_line += extra_command_line_arguments
-
         pattern = re.compile(r"([\"\'].+?[\"\'])|\s")
         return [x for y in cmd_line for x in re.split(pattern, y) if x]
 
     @property
     def venv_was_created(self):
-        return os.path.isdir(self.VENV_DIR.name)
+        return os.path.isdir(self.venv_dir)
 
-    def _create_venv(self):
+    def _create_venv(self, tmp_dir: str):
         """
         Creates the virtual environment for the example.
         """
-        self.VENV_DIR = TemporaryDirectory(prefix="venv_")
-        cmd_line = f"python -m venv {self.VENV_DIR.name}".split()
+        self.venv_dir = Path(tmp_dir) / "venv"
+        cmd_line = f"python -m venv {self.venv_dir}".split()
         p = subprocess.run(cmd_line)
         self.assertEqual(p.returncode, 0)
 
-    def _remove_venv(self):
-        """
-        Creates the virtual environment for the example.
-        """
-        if self.venv_was_created:
-            self.VENV_DIR.cleanup()
-
     def _get_poptorch_wheel_path(self, sdk_path: Optional[str] = None) -> str:
         """
         Retrieves the path for the poptorch wheel.
         """
         if sdk_path is None:
             sdk_path = os.environ["SDK_PATH"]
         paths = glob.glob(f"{sdk_path}/poptorch-*.whl")
@@ -355,15 +387,15 @@
     def _get_popart_enable_path(self, sdk_path: Optional[str] = None):
         return self._get_enable_path("popart", sdk_path=sdk_path)
 
     def _install_requirements(self, requirements_filename: Union[str, os.PathLike]):
         """
         Installs the necessary requirements to run the example if the provided file exists, otherwise does nothing.
         """
-        pip_name = f"{self.VENV_DIR.name}/bin/pip" if self.venv_was_created else "pip"
+        pip_name = f"{self.venv_dir}/bin/pip" if self.venv_was_created else "pip"
 
         # Update pip
         cmd_line = f"{pip_name} install --upgrade pip".split()
         p = subprocess.run(cmd_line)
         self.assertEqual(p.returncode, 0)
 
         # Install SDK
@@ -442,43 +474,45 @@
         "--preprocessing_num_workers 16",
     ]
 
     def _create_command_line(
         self,
         script: str,
         model_name: str,
-        ipu_config_name: str,
+        ipu_config: Union[str, IPUConfig],
         output_dir: str,
         task: Optional[str] = None,
         dataset_config_name: Optional[str] = None,
         do_eval: bool = True,
         lr: float = 1e-4,
         train_batch_size: int = 1,
         eval_batch_size: int = 1,
         num_epochs: int = 2,
+        max_steps: int = -1,
         inference_device_iterations: int = 6,
         gradient_accumulation_steps: int = 64,
         extra_command_line_arguments: Optional[List[str]] = None,
     ) -> List[str]:
         if extra_command_line_arguments is None:
             extra_command_line_arguments = []
         if "t5" in model_name:
             extra_command_line_arguments.append("--source_prefix 'summarize: '")
         return super()._create_command_line(
             script,
             model_name,
-            ipu_config_name,
+            ipu_config,
             output_dir,
             task=task,
             dataset_config_name=dataset_config_name,
             do_eval=do_eval,
             lr=lr,
             train_batch_size=train_batch_size,
             eval_batch_size=eval_batch_size,
             num_epochs=num_epochs,
+            max_steps=max_steps,
             inference_device_iterations=inference_device_iterations,
             gradient_accumulation_steps=gradient_accumulation_steps,
             extra_command_line_arguments=extra_command_line_arguments,
         )
 
 
 class TranslationExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_translation"):
@@ -500,43 +534,45 @@
         "--preprocessing_num_workers 16",
     ]
 
     def _create_command_line(
         self,
         script: str,
         model_name: str,
-        ipu_config_name: str,
+        ipu_config: Union[str, IPUConfig],
         output_dir: str,
         task: Optional[str] = None,
         dataset_config_name: Optional[str] = None,
         do_eval: bool = True,
         lr: float = 1e-4,
         train_batch_size: int = 1,
         eval_batch_size: int = 1,
         num_epochs: int = 2,
+        max_steps: int = -1,
         inference_device_iterations: int = 6,
         gradient_accumulation_steps: int = 64,
         extra_command_line_arguments: Optional[List[str]] = None,
     ) -> List[str]:
         if extra_command_line_arguments is None:
             extra_command_line_arguments = []
         if "t5" in model_name:
             extra_command_line_arguments.append("--source_prefix 'translate English to Romanian: '")
         return super()._create_command_line(
             script,
             model_name,
-            ipu_config_name,
+            ipu_config,
             output_dir,
             task=task,
             dataset_config_name=dataset_config_name,
             do_eval=do_eval,
             lr=lr,
             train_batch_size=train_batch_size,
             eval_batch_size=eval_batch_size,
             num_epochs=num_epochs,
+            max_steps=max_steps,
             inference_device_iterations=inference_device_iterations,
             gradient_accumulation_steps=gradient_accumulation_steps,
             extra_command_line_arguments=extra_command_line_arguments,
         )
 
 
 class ImageClassificationExampleTester(
```

### Comparing `optimum-graphcore-0.7.0/tests/test_examples_match_transformers.py` & `optimum-graphcore-0.7.1/tests/test_examples_match_transformers.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/tests/test_ipu_configuration.py` & `optimum-graphcore-0.7.1/tests/test_ipu_configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/tests/test_modeling_common.py` & `optimum-graphcore-0.7.1/tests/test_modeling_common.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/tests/test_modeling_utils.py` & `optimum-graphcore-0.7.1/tests/test_modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/tests/test_pipelined_models.py` & `optimum-graphcore-0.7.1/tests/test_pipelined_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,19 +90,22 @@
     models_to_test = []
     for pretrained_class, pipelined_class in _PRETRAINED_TO_PIPELINED_REGISTRY.items():
         test_name = f"{pretrained_class.__name__}"
         config_class = find_config_class_from_pretrained_class(pretrained_class)
         names = model_to_test_names[REVERSE_CONFIG_MAPPING[config_class]]
         if isinstance(names, dict):
             task = "ctc" if "CTC" in test_name else "default"
-            model_name_or_path, ipu_config_name_or_path = names.get(task, "default")
+            names = names.get(task, "default")
+            model_name_or_path = names.model
+            ipu_config = names.ipu_config
         else:
-            model_name_or_path, ipu_config_name_or_path = names
+            model_name_or_path = names.model
+            ipu_config = names.ipu_config
         models_to_test.append(
-            (test_name, model_name_or_path, ipu_config_name_or_path, pretrained_class, pipelined_class, config_class)
+            (test_name, model_name_or_path, ipu_config, pretrained_class, pipelined_class, config_class)
         )
     return models_to_test
 
 
 MODELS_TO_TEST = _get_models_to_test(MODELS_TO_TEST_MAPPING)
 
 
@@ -176,25 +179,40 @@
             inputs = extractor(
                 "This is a test to check that pretrained and pipeline model outputs match.", return_tensors="pt"
             )
         return inputs
 
     @parameterized.expand(MODELS_TO_TEST)
     def test_pretrained_and_pipelined_models_match(
-        self, test_name, model_name_or_path, ipu_config_name_or_path, pretrained_class, pipelined_class, config_class
+        self, test_name, model_name_or_path, ipu_config, pretrained_class, pipelined_class, config_class
     ):
         config = config_class.from_pretrained(model_name_or_path)
-        ipu_config = IPUConfig.from_pretrained(ipu_config_name_or_path)
+        if isinstance(ipu_config, str):
+            ipu_config = IPUConfig.from_pretrained(ipu_config)
+
+        # Serialized layers split large modules into submodules with the result
+        # aggregated/combined across submodules. Since torch uses intra-op parallelism,
+        # intermediate thread results may be different when comparing computation on a single module
+        # vs the serialized module. Since floating point addition is sensitive to the order of accumulation of
+        # intermediate results, results from serialized layers will be marginally different from the original layer.
+        # The code below turns off intra-op parallelism since the aim of this test is to test functional correctnesss
+        model_using_serialized_splits_per_ipu = (
+            ipu_config.serialized_embedding_splits_per_ipu or ipu_config.serialized_projection_splits_per_ipu
+        )
+        if model_using_serialized_splits_per_ipu:
+            torch_original_intra_op_thread_count = torch.get_num_threads()
+            torch.set_num_threads(1)
+
         pretrained_model = pretrained_class(config).eval()
         pipelined_model = pipelined_class.from_transformers(pretrained_model, ipu_config).eval()
 
         inputs = self._generate_input_for_model_class(model_name_or_path, pretrained_class)
         pretrained_model_outputs = pretrained_model(**inputs, return_dict=True)
 
-        pipelined_model.parallelize()
+        pipelined_model.parallelize(**ipu_config.inference_parallelize_kwargs)
         pipelined_model_outputs = pipelined_model.forward(**inputs, return_dict=True)
         for idx, k in enumerate(pretrained_model_outputs.keys()):
             pretrained_output, pipelined_output = pretrained_model_outputs[k], pipelined_model_outputs[k]
             # Handle tuple outputs. Outputs such as past_key_values are returned as tuples.
             if isinstance(pretrained_output, tuple):
                 for x, y in zip(pretrained_output, pipelined_output):
                     if isinstance(x, tuple):
@@ -236,30 +254,35 @@
 
             else:
                 self.assertTrue(
                     torch.allclose(pretrained_output, pipelined_output, atol=1e-5),
                     f"Pretrained and pipelined model {idx}th outputs do not match, max difference = {(pretrained_output - pipelined_output).abs().max()}",
                 )
 
+        if model_using_serialized_splits_per_ipu:
+            torch.set_num_threads(torch_original_intra_op_thread_count)
+
     @parameterized.expand(MODELS_TO_TEST)
     def test_parallelize_deparallelize(
-        self, test_name, model_name_or_path, ipu_config_name_or_path, pretrained_class, pipelined_class, config_class
+        self, test_name, model_name_or_path, ipu_config, pretrained_class, pipelined_class, config_class
     ):
-        ipu_config = IPUConfig.from_pretrained(ipu_config_name_or_path)
+        if isinstance(ipu_config, str):
+            ipu_config = IPUConfig.from_pretrained(ipu_config)
+
         model = pipelined_class.from_pretrained_transformers(model_name_or_path, ipu_config)
 
         # Remove the weight-norm hook, if present, because it doesn't work with deepcopy
         # https://github.com/pytorch/pytorch/issues/28594
         for module in model.modules():
             for _, hook in module._forward_pre_hooks.items():
                 if isinstance(hook, WeightNorm):
                     delattr(module, hook.name)
 
         modules_before = copy.deepcopy(model).modules()
-        model.parallelize()
+        model.parallelize(**ipu_config.parallelize_kwargs)
         model.deparallelize()
         modules_after = copy.deepcopy(model).modules()
         # Confirm that parallelize then deparallelize won't change the model's modules
         for mod_before, mod_after in zip(modules_before, modules_after):
             self.assertEqual(type(mod_before), type(mod_after))
 
-        model.parallelize()
+        model.parallelize(**ipu_config.parallelize_kwargs)
```

### Comparing `optimum-graphcore-0.7.0/tests/test_trainer.py` & `optimum-graphcore-0.7.1/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.7.0/tests/test_trainer_seq2seq.py` & `optimum-graphcore-0.7.1/tests/test_trainer_seq2seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
             batch["decoder_input_ids"] = outputs.input_ids
             batch["labels"] = outputs.input_ids.copy()
             batch["labels"] = [
                 [-100 if token == tokenizer.pad_token_id else token for token in labels] for labels in batch["labels"]
             ]
             batch["decoder_attention_mask"] = outputs.attention_mask
 
-            assert all([len(x) == 512 for x in inputs.input_ids])
-            assert all([len(x) == 128 for x in outputs.input_ids])
+            assert all(len(x) == 512 for x in inputs.input_ids)
+            assert all(len(x) == 128 for x in outputs.input_ids)
 
             return batch
 
         def _compute_metrics(pred):
             labels_ids = pred.label_ids
             pred_ids = pred.predictions
```


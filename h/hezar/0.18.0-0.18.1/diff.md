# Comparing `tmp/hezar-0.18.0.tar.gz` & `tmp/hezar-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.18.0.tar", max compression
+gzip compressed data, was "hezar-0.18.1.tar", max compression
```

## Comparing `hezar-0.18.0.tar` & `hezar-0.18.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1065 2023-07-30 08:30:20.049396 hezar-0.18.0/LICENSE
--rw-r--r--   0        0        0     4309 2023-07-30 08:30:20.049396 hezar-0.18.0/README.md
--rw-r--r--   0        0        0      261 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/__init__.py
--rw-r--r--   0        0        0     5384 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/builders.py
--rw-r--r--   0        0        0    11117 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/configs.py
--rw-r--r--   0        0        0     2068 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/__init__.py
--rw-r--r--   0        0        0     6364 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0      223 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4502 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3627 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      282 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1604 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1676 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1634 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11760 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/model.py
--rw-r--r--   0        0        0      152 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     3971 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      877 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3530 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     3666 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3809 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      142 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     3603 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/normalizer.py
--rw-r--r--   0        0        0     3852 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      231 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    19353 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8674 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2643 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2243 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    17687 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      161 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5614 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/core_utils.py
--rw-r--r--   0        0        0     3660 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1648 2023-07-30 08:30:20.053396 hezar-0.18.0/pyproject.toml
--rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 hezar-0.18.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-31 06:23:56.132397 hezar-0.18.1/LICENSE
+-rw-r--r--   0        0        0     4309 2023-07-31 06:23:56.132397 hezar-0.18.1/README.md
+-rw-r--r--   0        0        0      260 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/__init__.py
+-rw-r--r--   0        0        0     5336 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/builders.py
+-rw-r--r--   0        0        0    11117 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/configs.py
+-rw-r--r--   0        0        0     2068 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6364 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      223 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4502 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3627 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      282 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1604 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1676 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1634 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11760 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/model.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     3971 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      877 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3530 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     3666 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3809 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      142 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     3603 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/normalizer.py
+-rw-r--r--   0        0        0     3852 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      231 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    19353 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8828 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2643 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2243 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    17687 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      164 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5614 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0     3660 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/logging.py
+-rw-r--r--   0        0        0      936 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     1648 2023-07-31 06:23:56.140397 hezar-0.18.1/pyproject.toml
+-rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 hezar-0.18.1/PKG-INFO
```

### Comparing `hezar-0.18.0/LICENSE` & `hezar-0.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/README.md` & `hezar-0.18.1/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/builders.py` & `hezar-0.18.1/hezar/builders.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,20 @@
     DatasetConfig,
     EmbeddingConfig,
     MetricConfig,
     ModelConfig,
     PreprocessorConfig,
 )
 from .constants import SplitType
-from .registry import (  # noqa
-    datasets_registry,  # noqa
-    embeddings_registry,  # noqa
-    metrics_registry,  # noqa
-    models_registry,  # noqa
-    preprocessors_registry,  # noqa
+from .registry import (
+    datasets_registry,
+    embeddings_registry,
+    metrics_registry,
+    models_registry,
+    preprocessors_registry,
 )
 from .utils import snake_case
 
 
 __all__ = [
     "build_model",
     "build_dataset",
```

### Comparing `hezar-0.18.0/hezar/configs.py` & `hezar-0.18.1/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/constants.py` & `hezar-0.18.1/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/data/data_collators.py` & `hezar-0.18.1/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/data/datasets/dataset.py` & `hezar-0.18.1/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.18.1/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.18.1/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/data/utils/data_utils.py` & `hezar-0.18.1/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/embeddings/embedding.py` & `hezar-0.18.1/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/embeddings/fasttext.py` & `hezar-0.18.1/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/embeddings/word2vec.py` & `hezar-0.18.1/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/metrics/f1.py` & `hezar-0.18.1/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/metrics/metric.py` & `hezar-0.18.1/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/metrics/recall.py` & `hezar-0.18.1/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/metrics/seqeval.py` & `hezar-0.18.1/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.18.1/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.18.1/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.18.1/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.18.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.18.1/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.18.1/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/model.py` & `hezar-0.18.1/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.18.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.18.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.18.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.18.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.18.1/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.18.1/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.18.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.18.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.18.1/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.18.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/preprocessors/normalizer.py` & `hezar-0.18.1/hezar/preprocessors/normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/preprocessors/preprocessor.py` & `hezar-0.18.1/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.18.1/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.18.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.18.1/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.18.1/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/registry.py` & `hezar-0.18.1/hezar/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,20 @@
     "register_model",
     "register_preprocessor",
     "register_dataset",
     "register_embedding",
     "register_metric",
     "register_trainer",
     "Registry",
+    "models_registry",
+    "preprocessors_registry",
+    "datasets_registry",
+    "embeddings_registry",
+    "metrics_registry",
+    "trainers_registry",
 ]
 
 logger = get_logger(__name__)
 
 
 @dataclass
 class Registry:
```

### Comparing `hezar-0.18.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.18.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.18.1/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/trainers/trainer.py` & `hezar-0.18.1/hezar/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/trainers/trainer_utils.py` & `hezar-0.18.1/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/utils/common_utils.py` & `hezar-0.18.1/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/utils/core_utils.py` & `hezar-0.18.1/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/hezar/utils/hub_utils.py` & `hezar-0.18.1/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.0/pyproject.toml` & `hezar-0.18.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.18.0"
+version = "0.18.1"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.18.0/PKG-INFO` & `hezar-0.18.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.18.0
+Version: 0.18.1
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```


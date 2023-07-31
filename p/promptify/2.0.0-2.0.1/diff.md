# Comparing `tmp/promptify-2.0.0.tar.gz` & `tmp/promptify-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptify-2.0.0.tar", last modified: Sat Jul 29 16:16:01 2023, max compression
+gzip compressed data, was "promptify-2.0.1.tar", last modified: Mon Jul 31 04:45:12 2023, max compression
```

## Comparing `promptify-2.0.0.tar` & `promptify-2.0.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.808524 promptify-2.0.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-29 16:15:49.000000 promptify-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-29 16:16:01.807525 promptify-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6965 2023-07-29 16:15:49.000000 promptify-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.789523 promptify-2.0.0/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/benchmarks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.790523 promptify-2.0.0/examples/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-07-29 16:15:49.000000 promptify-2.0.0/examples/medical_ner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.790523 promptify-2.0.0/promptify/
--rw-r--r--   0 root         (0) root         (0)      776 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.791523 promptify-2.0.0/promptify/data/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.791523 promptify-2.0.0/promptify/data/text2text/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/data/text2text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.791523 promptify-2.0.0/promptify/data/text2text/en/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/data/text2text/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.791523 promptify-2.0.0/promptify/databases/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/databases/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.791523 promptify-2.0.0/promptify/embeddings/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/embeddings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.792523 promptify-2.0.0/promptify/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.792523 promptify-2.0.0/promptify/models/text2image/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2image/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.792523 promptify-2.0.0/promptify/models/text2text/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.793523 promptify-2.0.0/promptify/models/text2text/api/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2text/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2text/api/anthropic.py
--rw-r--r--   0 root         (0) root         (0)     5681 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2text/api/azure_openai.py
--rw-r--r--   0 root         (0) root         (0)    12087 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2text/api/base_model.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2text/api/cohere.py
--rw-r--r--   0 root         (0) root         (0)     5631 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2text/api/hub_model.py
--rw-r--r--   0 root         (0) root         (0)     4433 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2text/api/mock_model.py
--rw-r--r--   0 root         (0) root         (0)     6359 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2text/api/openai_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.793523 promptify-2.0.0/promptify/models/text2text/inference/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/models/text2text/inference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.794523 promptify-2.0.0/promptify/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12197 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/parser/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.794523 promptify-2.0.0/promptify/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3542 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/pipelines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.794523 promptify-2.0.0/promptify/plugins/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.795523 promptify-2.0.0/promptify/prompter/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1870 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompter/conversation_logger.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompter/nlp_prompter.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompter/prompt_cache.py
--rw-r--r--   0 root         (0) root         (0)     5401 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompter/template_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.795523 promptify-2.0.0/promptify/prompts/
--rw-r--r--   0 root         (0) root         (0)        2 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.795523 promptify-2.0.0/promptify/prompts/text2image/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2image/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.795523 promptify-2.0.0/promptify/prompts/text2text/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.796523 promptify-2.0.0/promptify/prompts/text2text/binary_classification/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/binary_classification/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/binary_classification/binary_classification.jinja
--rw-r--r--   0 root         (0) root         (0)     1549 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/binary_classification/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.797523 promptify-2.0.0/promptify/prompts/text2text/explain/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/explain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/explain/explain.jinja
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/explain/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.798524 promptify-2.0.0/promptify/prompts/text2text/multiclass_classification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/multiclass_classification/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/multiclass_classification/metadata.json
--rw-r--r--   0 root         (0) root         (0)      610 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/multiclass_classification/multiclass_classification.jinja
--rw-r--r--   0 root         (0) root         (0)      610 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/multiclass_classification/multiclass_gpt.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.799524 promptify-2.0.0/promptify/prompts/text2text/multilabel_classification/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/multilabel_classification/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/multilabel_classification/metadata.json
--rw-r--r--   0 root         (0) root         (0)     1067 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/multilabel_classification/multilabel_classification.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.799524 promptify-2.0.0/promptify/prompts/text2text/ner/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/ner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/ner/metadata.json
--rw-r--r--   0 root         (0) root         (0)     1923 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/ner/ner_openai.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.800524 promptify-2.0.0/promptify/prompts/text2text/qa/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/qa/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/qa/metadata.json
--rw-r--r--   0 root         (0) root         (0)      864 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/qa/qa.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.801524 promptify-2.0.0/promptify/prompts/text2text/qa_gen/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/qa_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/qa_gen/metadata.json
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/qa_gen/qa_gen.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.801524 promptify-2.0.0/promptify/prompts/text2text/relation_extraction/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/relation_extraction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/relation_extraction/metadata.json
--rw-r--r--   0 root         (0) root         (0)     1056 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/relation_extraction/relation_extraction.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.802524 promptify-2.0.0/promptify/prompts/text2text/sql_writer/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/sql_writer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/sql_writer/metadata.json
--rw-r--r--   0 root         (0) root         (0)      867 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/sql_writer/sql_writer_gpt.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.802524 promptify-2.0.0/promptify/prompts/text2text/summary/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/summary/summary.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.803524 promptify-2.0.0/promptify/prompts/text2text/tabular_extractor/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/tabular_extractor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/tabular_extractor/metadata.json
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/tabular_extractor/tabular_extractor_gpt.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.804524 promptify-2.0.0/promptify/prompts/text2text/text_normalization/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/text_normalization/__init__.py
--rw-r--r--   0 root         (0) root         (0)      756 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/text_normalization/text_normalization_draft.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.804524 promptify-2.0.0/promptify/prompts/text2text/topic_modelling/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/topic_modelling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1478 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/prompts/text2text/topic_modelling/topic_modeling_draft.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.805524 promptify-2.0.0/promptify/utils/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2424 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/utils/conversation_utils.py
--rw-r--r--   0 root         (0) root         (0)      532 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/utils/data_utils.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-07-29 16:15:49.000000 promptify-2.0.0/promptify/utils/file_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.791523 promptify-2.0.0/promptify.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-29 16:16:01.000000 promptify-2.0.0/promptify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4059 2023-07-29 16:16:01.000000 promptify-2.0.0/promptify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:16:01.000000 promptify-2.0.0/promptify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-29 16:16:01.000000 promptify-2.0.0/promptify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-29 16:16:01.000000 promptify-2.0.0/promptify.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 16:16:01.808524 promptify-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1330 2023-07-29 16:15:49.000000 promptify-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.805524 promptify-2.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.805524 promptify-2.0.0/tests/unit_tests/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/tests/unit_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.806524 promptify-2.0.0/tests/unit_tests/models/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/tests/unit_tests/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-07-29 16:15:49.000000 promptify-2.0.0/tests/unit_tests/models/test_base_model.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-29 16:15:49.000000 promptify-2.0.0/tests/unit_tests/models/test_hf_model.py
--rw-r--r--   0 root         (0) root         (0)     7580 2023-07-29 16:15:49.000000 promptify-2.0.0/tests/unit_tests/models/test_openai_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.806524 promptify-2.0.0/tests/unit_tests/parser/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/tests/unit_tests/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5427 2023-07-29 16:15:49.000000 promptify-2.0.0/tests/unit_tests/parser/test_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:16:01.807525 promptify-2.0.0/tests/unit_tests/prompter/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:15:49.000000 promptify-2.0.0/tests/unit_tests/prompter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4179 2023-07-29 16:15:49.000000 promptify-2.0.0/tests/unit_tests/prompter/test_prompter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.227097 promptify-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-31 04:45:06.000000 promptify-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-31 04:45:12.227097 promptify-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-07-31 04:45:06.000000 promptify-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.206095 promptify-2.0.1/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/benchmarks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.206095 promptify-2.0.1/examples/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-31 04:45:06.000000 promptify-2.0.1/examples/medical_ner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.207095 promptify-2.0.1/promptify/
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.208095 promptify-2.0.1/promptify/data/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.209095 promptify-2.0.1/promptify/data/text2text/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/data/text2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.209095 promptify-2.0.1/promptify/data/text2text/en/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/data/text2text/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.209095 promptify-2.0.1/promptify/databases/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/databases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.210095 promptify-2.0.1/promptify/embeddings/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/embeddings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.210095 promptify-2.0.1/promptify/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.210095 promptify-2.0.1/promptify/models/text2image/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2image/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.210095 promptify-2.0.1/promptify/models/text2text/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.212095 promptify-2.0.1/promptify/models/text2text/api/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2text/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2text/api/anthropic.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2text/api/azure_openai.py
+-rw-r--r--   0 root         (0) root         (0)    12087 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2text/api/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2text/api/cohere.py
+-rw-r--r--   0 root         (0) root         (0)     5631 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2text/api/hub_model.py
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2text/api/mock_model.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2text/api/openai_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.212095 promptify-2.0.1/promptify/models/text2text/inference/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/models/text2text/inference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.212095 promptify-2.0.1/promptify/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12197 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/parser/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.212095 promptify-2.0.1/promptify/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/pipelines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.212095 promptify-2.0.1/promptify/plugins/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.213096 promptify-2.0.1/promptify/prompter/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompter/conversation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompter/nlp_prompter.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompter/prompt_cache.py
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompter/template_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.214096 promptify-2.0.1/promptify/prompts/
+-rw-r--r--   0 root         (0) root         (0)        2 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.214096 promptify-2.0.1/promptify/prompts/text2image/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2image/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.214096 promptify-2.0.1/promptify/prompts/text2text/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.214096 promptify-2.0.1/promptify/prompts/text2text/binary_classification/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/binary_classification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/binary_classification/binary_classification.jinja
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/binary_classification/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.215096 promptify-2.0.1/promptify/prompts/text2text/explain/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/explain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/explain/explain.jinja
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/explain/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.216096 promptify-2.0.1/promptify/prompts/text2text/multiclass_classification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/multiclass_classification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/multiclass_classification/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      610 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/multiclass_classification/multiclass_classification.jinja
+-rw-r--r--   0 root         (0) root         (0)      610 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/multiclass_classification/multiclass_gpt.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.216096 promptify-2.0.1/promptify/prompts/text2text/multilabel_classification/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/multilabel_classification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/multilabel_classification/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/multilabel_classification/multilabel_classification.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.217096 promptify-2.0.1/promptify/prompts/text2text/ner/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/ner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/ner/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/ner/ner_openai.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.217096 promptify-2.0.1/promptify/prompts/text2text/qa/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/qa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/qa/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      864 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/qa/qa.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.218096 promptify-2.0.1/promptify/prompts/text2text/qa_gen/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/qa_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/qa_gen/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/qa_gen/qa_gen.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.218096 promptify-2.0.1/promptify/prompts/text2text/relation_extraction/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/relation_extraction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/relation_extraction/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/relation_extraction/relation_extraction.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.219096 promptify-2.0.1/promptify/prompts/text2text/sql_writer/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/sql_writer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/sql_writer/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      867 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/sql_writer/sql_writer_gpt.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.219096 promptify-2.0.1/promptify/prompts/text2text/summary/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/summary/summary.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.220096 promptify-2.0.1/promptify/prompts/text2text/tabular_extractor/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/tabular_extractor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/tabular_extractor/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/tabular_extractor/tabular_extractor_gpt.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.220096 promptify-2.0.1/promptify/prompts/text2text/text_normalization/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/text_normalization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/text_normalization/text_normalization_draft.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.221096 promptify-2.0.1/promptify/prompts/text2text/topic_modelling/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/topic_modelling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/prompts/text2text/topic_modelling/topic_modeling_draft.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.222096 promptify-2.0.1/promptify/utils/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/utils/conversation_utils.py
+-rw-r--r--   0 root         (0) root         (0)      532 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/utils/data_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-07-31 04:45:06.000000 promptify-2.0.1/promptify/utils/file_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.208095 promptify-2.0.1/promptify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-31 04:45:11.000000 promptify-2.0.1/promptify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4059 2023-07-31 04:45:11.000000 promptify-2.0.1/promptify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:11.000000 promptify-2.0.1/promptify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-31 04:45:11.000000 promptify-2.0.1/promptify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-31 04:45:11.000000 promptify-2.0.1/promptify.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 04:45:12.227097 promptify-2.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-07-31 04:45:06.000000 promptify-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.223096 promptify-2.0.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.223096 promptify-2.0.1/tests/unit_tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/tests/unit_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.225097 promptify-2.0.1/tests/unit_tests/models/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/tests/unit_tests/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-07-31 04:45:06.000000 promptify-2.0.1/tests/unit_tests/models/test_base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-31 04:45:06.000000 promptify-2.0.1/tests/unit_tests/models/test_hf_model.py
+-rw-r--r--   0 root         (0) root         (0)     7580 2023-07-31 04:45:06.000000 promptify-2.0.1/tests/unit_tests/models/test_openai_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.226097 promptify-2.0.1/tests/unit_tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/tests/unit_tests/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5427 2023-07-31 04:45:06.000000 promptify-2.0.1/tests/unit_tests/parser/test_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:45:12.226097 promptify-2.0.1/tests/unit_tests/prompter/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:45:06.000000 promptify-2.0.1/tests/unit_tests/prompter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-07-31 04:45:06.000000 promptify-2.0.1/tests/unit_tests/prompter/test_prompter.py
```

### Comparing `promptify-2.0.0/LICENSE` & `promptify-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/PKG-INFO` & `promptify-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptify
-Version: 2.0.0
+Version: 2.0.1
 Summary: Use GPT or other prompt based models to get structured output
 Home-page: https://github.com/promptslab/Promptify
 Author: monk1337
 Maintainer: The promptslab team with the help of all our contributors
 License: Apache
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_6rz3dpbg_/tmp60f5untp_TarContainer/0/2", line 109, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_6rz3dpbg_/tmp60f5untp_TarContainer/0/2", line 109, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptify Version: 2.0.0 Summary: Use GPT or other
+Metadata-Version: 2.1 Name: promptify Version: 2.0.1 Summary: Use GPT or other
 prompt based models to get structured output Home-page: https://github.com/
 promptslab/Promptify Author: monk1337 Maintainer: The promptslab team with the
 help of all our contributors License: Apache Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE
  [https://raw.githubusercontent.com/promptslab/Promptify/main/assets/logo.png]
                             ****** Promptify ******
```

### Comparing `promptify-2.0.0/README.md` & `promptify-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/examples/medical_ner.py` & `promptify-2.0.1/examples/medical_ner.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/__init__.py` & `promptify-2.0.1/promptify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.4"
+__version__ = "2.0.1"
 from .parser.parser import Parser
 from .prompter.nlp_prompter import Prompter
 from .prompter.prompt_cache import PromptCache
 from .prompter.template_loader import TemplateLoader
 from .prompter.conversation_logger import ConversationLogger
 from .models.text2text.api.openai_models import OpenAI
 from .models.text2text.api.anthropic import AnthropicModel
```

### Comparing `promptify-2.0.0/promptify/models/text2text/api/anthropic.py` & `promptify-2.0.1/promptify/models/text2text/api/anthropic.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/models/text2text/api/azure_openai.py` & `promptify-2.0.1/promptify/models/text2text/api/azure_openai.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/models/text2text/api/base_model.py` & `promptify-2.0.1/promptify/models/text2text/api/base_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/models/text2text/api/cohere.py` & `promptify-2.0.1/promptify/models/text2text/api/cohere.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/models/text2text/api/hub_model.py` & `promptify-2.0.1/promptify/models/text2text/api/hub_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/models/text2text/api/mock_model.py` & `promptify-2.0.1/promptify/models/text2text/api/mock_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/models/text2text/api/openai_models.py` & `promptify-2.0.1/promptify/models/text2text/api/openai_models.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/parser/parser.py` & `promptify-2.0.1/promptify/parser/parser.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/pipelines/__init__.py` & `promptify-2.0.1/promptify/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompter/conversation_logger.py` & `promptify-2.0.1/promptify/prompter/conversation_logger.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompter/nlp_prompter.py` & `promptify-2.0.1/promptify/prompter/nlp_prompter.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompter/prompt_cache.py` & `promptify-2.0.1/promptify/prompter/prompt_cache.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompter/template_loader.py` & `promptify-2.0.1/promptify/prompter/template_loader.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/binary_classification/binary_classification.jinja` & `promptify-2.0.1/promptify/prompts/text2text/binary_classification/binary_classification.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/binary_classification/metadata.json` & `promptify-2.0.1/promptify/prompts/text2text/binary_classification/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/explain/explain.jinja` & `promptify-2.0.1/promptify/prompts/text2text/explain/explain.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/explain/metadata.json` & `promptify-2.0.1/promptify/prompts/text2text/explain/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/multiclass_classification/metadata.json` & `promptify-2.0.1/promptify/prompts/text2text/multiclass_classification/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/multiclass_classification/multiclass_classification.jinja` & `promptify-2.0.1/promptify/prompts/text2text/multiclass_classification/multiclass_classification.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/multiclass_classification/multiclass_gpt.jinja` & `promptify-2.0.1/promptify/prompts/text2text/multiclass_classification/multiclass_gpt.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/multilabel_classification/metadata.json` & `promptify-2.0.1/promptify/prompts/text2text/multilabel_classification/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/multilabel_classification/multilabel_classification.jinja` & `promptify-2.0.1/promptify/prompts/text2text/multilabel_classification/multilabel_classification.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/ner/metadata.json` & `promptify-2.0.1/promptify/prompts/text2text/ner/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/ner/ner_openai.jinja` & `promptify-2.0.1/promptify/prompts/text2text/ner/ner_openai.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/qa/qa.jinja` & `promptify-2.0.1/promptify/prompts/text2text/qa/qa.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/qa_gen/qa_gen.jinja` & `promptify-2.0.1/promptify/prompts/text2text/qa_gen/qa_gen.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/relation_extraction/metadata.json` & `promptify-2.0.1/promptify/prompts/text2text/relation_extraction/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/relation_extraction/relation_extraction.jinja` & `promptify-2.0.1/promptify/prompts/text2text/relation_extraction/relation_extraction.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/sql_writer/metadata.json` & `promptify-2.0.1/promptify/prompts/text2text/sql_writer/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/sql_writer/sql_writer_gpt.jinja` & `promptify-2.0.1/promptify/prompts/text2text/sql_writer/sql_writer_gpt.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/summary/summary.jinja` & `promptify-2.0.1/promptify/prompts/text2text/summary/summary.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/tabular_extractor/metadata.json` & `promptify-2.0.1/promptify/prompts/text2text/tabular_extractor/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/text_normalization/text_normalization_draft.jinja` & `promptify-2.0.1/promptify/prompts/text2text/text_normalization/text_normalization_draft.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/prompts/text2text/topic_modelling/topic_modeling_draft.jinja` & `promptify-2.0.1/promptify/prompts/text2text/topic_modelling/topic_modeling_draft.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/utils/conversation_utils.py` & `promptify-2.0.1/promptify/utils/conversation_utils.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/utils/data_utils.py` & `promptify-2.0.1/promptify/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify/utils/file_utils.py` & `promptify-2.0.1/promptify/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/promptify.egg-info/PKG-INFO` & `promptify-2.0.1/promptify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptify
-Version: 2.0.0
+Version: 2.0.1
 Summary: Use GPT or other prompt based models to get structured output
 Home-page: https://github.com/promptslab/Promptify
 Author: monk1337
 Maintainer: The promptslab team with the help of all our contributors
 License: Apache
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_6rz3dpbg_/tmp60f5untp_TarContainer/0/113", line 109, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_6rz3dpbg_/tmp60f5untp_TarContainer/0/113", line 109, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptify Version: 2.0.0 Summary: Use GPT or other
+Metadata-Version: 2.1 Name: promptify Version: 2.0.1 Summary: Use GPT or other
 prompt based models to get structured output Home-page: https://github.com/
 promptslab/Promptify Author: monk1337 Maintainer: The promptslab team with the
 help of all our contributors License: Apache Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE
  [https://raw.githubusercontent.com/promptslab/Promptify/main/assets/logo.png]
                             ****** Promptify ******
```

### Comparing `promptify-2.0.0/promptify.egg-info/SOURCES.txt` & `promptify-2.0.1/promptify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/setup.py` & `promptify-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/tests/unit_tests/models/test_base_model.py` & `promptify-2.0.1/tests/unit_tests/models/test_base_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/tests/unit_tests/models/test_hf_model.py` & `promptify-2.0.1/tests/unit_tests/models/test_hf_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/tests/unit_tests/models/test_openai_model.py` & `promptify-2.0.1/tests/unit_tests/models/test_openai_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/tests/unit_tests/parser/test_parser.py` & `promptify-2.0.1/tests/unit_tests/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.0/tests/unit_tests/prompter/test_prompter.py` & `promptify-2.0.1/tests/unit_tests/prompter/test_prompter.py`

 * *Files identical despite different names*


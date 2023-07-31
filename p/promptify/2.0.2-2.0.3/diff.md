# Comparing `tmp/promptify-2.0.2.tar.gz` & `tmp/promptify-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptify-2.0.2.tar", last modified: Mon Jul 31 05:00:11 2023, max compression
+gzip compressed data, was "promptify-2.0.3.tar", last modified: Mon Jul 31 05:06:38 2023, max compression
```

## Comparing `promptify-2.0.2.tar` & `promptify-2.0.3.tar`

### file list

```diff
@@ -1,137 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.404384 promptify-2.0.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-31 05:00:01.000000 promptify-2.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-31 05:00:01.000000 promptify-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-31 05:00:11.404384 promptify-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6965 2023-07-31 05:00:01.000000 promptify-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.384382 promptify-2.0.2/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/benchmarks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.385382 promptify-2.0.2/examples/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-07-31 05:00:01.000000 promptify-2.0.2/examples/medical_ner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.385382 promptify-2.0.2/promptify/
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/VERSION
--rw-r--r--   0 root         (0) root         (0)      776 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.386382 promptify-2.0.2/promptify/data/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.386382 promptify-2.0.2/promptify/data/text2text/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/data/text2text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.387383 promptify-2.0.2/promptify/data/text2text/en/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/data/text2text/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.387383 promptify-2.0.2/promptify/databases/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/databases/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.387383 promptify-2.0.2/promptify/embeddings/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/embeddings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.387383 promptify-2.0.2/promptify/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.387383 promptify-2.0.2/promptify/models/text2image/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2image/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.387383 promptify-2.0.2/promptify/models/text2text/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.390383 promptify-2.0.2/promptify/models/text2text/api/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2text/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2text/api/anthropic.py
--rw-r--r--   0 root         (0) root         (0)     5681 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2text/api/azure_openai.py
--rw-r--r--   0 root         (0) root         (0)    12087 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2text/api/base_model.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2text/api/cohere.py
--rw-r--r--   0 root         (0) root         (0)     5631 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2text/api/hub_model.py
--rw-r--r--   0 root         (0) root         (0)     4433 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2text/api/mock_model.py
--rw-r--r--   0 root         (0) root         (0)     6359 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2text/api/openai_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.390383 promptify-2.0.2/promptify/models/text2text/inference/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/models/text2text/inference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.391383 promptify-2.0.2/promptify/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12197 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/parser/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.391383 promptify-2.0.2/promptify/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3542 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/pipelines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.391383 promptify-2.0.2/promptify/plugins/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.392383 promptify-2.0.2/promptify/prompter/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1870 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompter/conversation_logger.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompter/nlp_prompter.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompter/prompt_cache.py
--rw-r--r--   0 root         (0) root         (0)     5401 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompter/template_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.392383 promptify-2.0.2/promptify/prompts/
--rw-r--r--   0 root         (0) root         (0)        2 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.393383 promptify-2.0.2/promptify/prompts/text2image/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2image/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.393383 promptify-2.0.2/promptify/prompts/text2text/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.394383 promptify-2.0.2/promptify/prompts/text2text/binary_classification/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/binary_classification/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/binary_classification/binary_classification.jinja
--rw-r--r--   0 root         (0) root         (0)     1549 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/binary_classification/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.394383 promptify-2.0.2/promptify/prompts/text2text/explain/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/explain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/explain/explain.jinja
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/explain/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.395383 promptify-2.0.2/promptify/prompts/text2text/multiclass_classification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/multiclass_classification/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/multiclass_classification/metadata.json
--rw-r--r--   0 root         (0) root         (0)      610 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/multiclass_classification/multiclass_classification.jinja
--rw-r--r--   0 root         (0) root         (0)      610 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/multiclass_classification/multiclass_gpt.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.396383 promptify-2.0.2/promptify/prompts/text2text/multilabel_classification/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/multilabel_classification/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/multilabel_classification/metadata.json
--rw-r--r--   0 root         (0) root         (0)     1067 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/multilabel_classification/multilabel_classification.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.396383 promptify-2.0.2/promptify/prompts/text2text/ner/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/ner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/ner/metadata.json
--rw-r--r--   0 root         (0) root         (0)     1923 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/ner/ner_openai.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.397383 promptify-2.0.2/promptify/prompts/text2text/qa/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/qa/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/qa/metadata.json
--rw-r--r--   0 root         (0) root         (0)      864 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/qa/qa.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.397383 promptify-2.0.2/promptify/prompts/text2text/qa_gen/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/qa_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/qa_gen/metadata.json
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/qa_gen/qa_gen.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.398383 promptify-2.0.2/promptify/prompts/text2text/relation_extraction/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/relation_extraction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/relation_extraction/metadata.json
--rw-r--r--   0 root         (0) root         (0)     1056 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/relation_extraction/relation_extraction.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.399383 promptify-2.0.2/promptify/prompts/text2text/sql_writer/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/sql_writer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/sql_writer/metadata.json
--rw-r--r--   0 root         (0) root         (0)      867 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/sql_writer/sql_writer_gpt.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.399383 promptify-2.0.2/promptify/prompts/text2text/summary/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/summary/summary.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.400383 promptify-2.0.2/promptify/prompts/text2text/tabular_extractor/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/tabular_extractor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/tabular_extractor/metadata.json
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/tabular_extractor/tabular_extractor_gpt.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.400383 promptify-2.0.2/promptify/prompts/text2text/text_normalization/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/text_normalization/__init__.py
--rw-r--r--   0 root         (0) root         (0)      756 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/text_normalization/text_normalization_draft.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.401383 promptify-2.0.2/promptify/prompts/text2text/topic_modelling/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/topic_modelling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1478 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/prompts/text2text/topic_modelling/topic_modeling_draft.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.401383 promptify-2.0.2/promptify/utils/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2424 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/utils/conversation_utils.py
--rw-r--r--   0 root         (0) root         (0)      532 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/utils/data_utils.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-07-31 05:00:01.000000 promptify-2.0.2/promptify/utils/file_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.386382 promptify-2.0.2/promptify.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-31 05:00:11.000000 promptify-2.0.2/promptify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4089 2023-07-31 05:00:11.000000 promptify-2.0.2/promptify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:11.000000 promptify-2.0.2/promptify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-31 05:00:11.000000 promptify-2.0.2/promptify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-31 05:00:11.000000 promptify-2.0.2/promptify.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 05:00:11.404384 promptify-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1330 2023-07-31 05:00:01.000000 promptify-2.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.401383 promptify-2.0.2/tests/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.402384 promptify-2.0.2/tests/unit_tests/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/tests/unit_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.402384 promptify-2.0.2/tests/unit_tests/models/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/tests/unit_tests/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-07-31 05:00:01.000000 promptify-2.0.2/tests/unit_tests/models/test_base_model.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-31 05:00:01.000000 promptify-2.0.2/tests/unit_tests/models/test_hf_model.py
--rw-r--r--   0 root         (0) root         (0)     7580 2023-07-31 05:00:01.000000 promptify-2.0.2/tests/unit_tests/models/test_openai_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.403384 promptify-2.0.2/tests/unit_tests/parser/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/tests/unit_tests/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5427 2023-07-31 05:00:01.000000 promptify-2.0.2/tests/unit_tests/parser/test_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:00:11.403384 promptify-2.0.2/tests/unit_tests/prompter/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:00:01.000000 promptify-2.0.2/tests/unit_tests/prompter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4179 2023-07-31 05:00:01.000000 promptify-2.0.2/tests/unit_tests/prompter/test_prompter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.345917 promptify-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-31 05:06:30.000000 promptify-2.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-31 05:06:30.000000 promptify-2.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-31 05:06:38.344917 promptify-2.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-07-31 05:06:30.000000 promptify-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.307914 promptify-2.0.3/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/benchmarks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.314915 promptify-2.0.3/examples/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-31 05:06:30.000000 promptify-2.0.3/examples/medical_ner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.318915 promptify-2.0.3/promptify/
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/VERSION
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.320915 promptify-2.0.3/promptify/data/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.320915 promptify-2.0.3/promptify/data/text2text/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/data/text2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.320915 promptify-2.0.3/promptify/data/text2text/en/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/data/text2text/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.321915 promptify-2.0.3/promptify/databases/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/databases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.321915 promptify-2.0.3/promptify/embeddings/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/embeddings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.321915 promptify-2.0.3/promptify/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.321915 promptify-2.0.3/promptify/models/text2image/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2image/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.322915 promptify-2.0.3/promptify/models/text2text/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.324916 promptify-2.0.3/promptify/models/text2text/api/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2text/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2text/api/anthropic.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2text/api/azure_openai.py
+-rw-r--r--   0 root         (0) root         (0)    12087 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2text/api/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2text/api/cohere.py
+-rw-r--r--   0 root         (0) root         (0)     5631 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2text/api/hub_model.py
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2text/api/mock_model.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2text/api/openai_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.325915 promptify-2.0.3/promptify/models/text2text/inference/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/models/text2text/inference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.325915 promptify-2.0.3/promptify/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12197 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/parser/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.326916 promptify-2.0.3/promptify/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/pipelines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.327916 promptify-2.0.3/promptify/plugins/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.329916 promptify-2.0.3/promptify/prompter/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompter/conversation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompter/nlp_prompter.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompter/prompt_cache.py
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompter/template_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.329916 promptify-2.0.3/promptify/prompts/
+-rw-r--r--   0 root         (0) root         (0)        2 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.329916 promptify-2.0.3/promptify/prompts/text2image/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2image/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.330916 promptify-2.0.3/promptify/prompts/text2text/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.331916 promptify-2.0.3/promptify/prompts/text2text/binary_classification/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/binary_classification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/binary_classification/binary_classification.jinja
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/binary_classification/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.331916 promptify-2.0.3/promptify/prompts/text2text/explain/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/explain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/explain/explain.jinja
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/explain/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.332916 promptify-2.0.3/promptify/prompts/text2text/multiclass_classification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/multiclass_classification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/multiclass_classification/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      610 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/multiclass_classification/multiclass_classification.jinja
+-rw-r--r--   0 root         (0) root         (0)      610 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/multiclass_classification/multiclass_gpt.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.333916 promptify-2.0.3/promptify/prompts/text2text/multilabel_classification/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/multilabel_classification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/multilabel_classification/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/multilabel_classification/multilabel_classification.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.334916 promptify-2.0.3/promptify/prompts/text2text/ner/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/ner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/ner/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/ner/ner_openai.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.335916 promptify-2.0.3/promptify/prompts/text2text/qa/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/qa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/qa/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      864 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/qa/qa.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.336916 promptify-2.0.3/promptify/prompts/text2text/qa_gen/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/qa_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/qa_gen/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/qa_gen/qa_gen.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.337916 promptify-2.0.3/promptify/prompts/text2text/relation_extraction/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/relation_extraction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/relation_extraction/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/relation_extraction/relation_extraction.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.337916 promptify-2.0.3/promptify/prompts/text2text/sql_writer/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/sql_writer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/sql_writer/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      867 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/sql_writer/sql_writer_gpt.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.338916 promptify-2.0.3/promptify/prompts/text2text/summary/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/summary/summary.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.339917 promptify-2.0.3/promptify/prompts/text2text/tabular_extractor/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/tabular_extractor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/tabular_extractor/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/tabular_extractor/tabular_extractor_gpt.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.339917 promptify-2.0.3/promptify/prompts/text2text/text_normalization/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/text_normalization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/text_normalization/text_normalization_draft.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.340916 promptify-2.0.3/promptify/prompts/text2text/topic_modelling/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/topic_modelling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/prompts/text2text/topic_modelling/topic_modeling_draft.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.341917 promptify-2.0.3/promptify/utils/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/utils/conversation_utils.py
+-rw-r--r--   0 root         (0) root         (0)      532 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/utils/data_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-07-31 05:06:30.000000 promptify-2.0.3/promptify/utils/file_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.320915 promptify-2.0.3/promptify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-31 05:06:37.000000 promptify-2.0.3/promptify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-07-31 05:06:37.000000 promptify-2.0.3/promptify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:37.000000 promptify-2.0.3/promptify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-31 05:06:37.000000 promptify-2.0.3/promptify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-31 05:06:37.000000 promptify-2.0.3/promptify.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-31 05:06:30.000000 promptify-2.0.3/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2023-07-31 05:06:30.000000 promptify-2.0.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 05:06:38.345917 promptify-2.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-07-31 05:06:30.000000 promptify-2.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.341917 promptify-2.0.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.342917 promptify-2.0.3/tests/unit_tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/tests/unit_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.343917 promptify-2.0.3/tests/unit_tests/models/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/tests/unit_tests/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-07-31 05:06:30.000000 promptify-2.0.3/tests/unit_tests/models/test_base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-31 05:06:30.000000 promptify-2.0.3/tests/unit_tests/models/test_hf_model.py
+-rw-r--r--   0 root         (0) root         (0)     7580 2023-07-31 05:06:30.000000 promptify-2.0.3/tests/unit_tests/models/test_openai_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.343917 promptify-2.0.3/tests/unit_tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/tests/unit_tests/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5427 2023-07-31 05:06:30.000000 promptify-2.0.3/tests/unit_tests/parser/test_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:06:38.344917 promptify-2.0.3/tests/unit_tests/prompter/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:06:30.000000 promptify-2.0.3/tests/unit_tests/prompter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-07-31 05:06:30.000000 promptify-2.0.3/tests/unit_tests/prompter/test_prompter.py
```

### Comparing `promptify-2.0.2/LICENSE` & `promptify-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/PKG-INFO` & `promptify-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptify
-Version: 2.0.2
+Version: 2.0.3
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

 * *File "/tmp/diffoscope_psgtamyl_/tmpiv4uj_o1_TarContainer/0/3", line 109, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_psgtamyl_/tmpiv4uj_o1_TarContainer/0/3", line 109, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptify Version: 2.0.2 Summary: Use GPT or other
+Metadata-Version: 2.1 Name: promptify Version: 2.0.3 Summary: Use GPT or other
 prompt based models to get structured output Home-page: https://github.com/
 promptslab/Promptify Author: monk1337 Maintainer: The promptslab team with the
 help of all our contributors License: Apache Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE
  [https://raw.githubusercontent.com/promptslab/Promptify/main/assets/logo.png]
                             ****** Promptify ******
```

### Comparing `promptify-2.0.2/README.md` & `promptify-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/examples/medical_ner.py` & `promptify-2.0.3/examples/medical_ner.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/__init__.py` & `promptify-2.0.3/promptify/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 from .parser.parser import Parser
 from .prompter.nlp_prompter import Prompter
 from .prompter.prompt_cache import PromptCache
 from .prompter.template_loader import TemplateLoader
 from .prompter.conversation_logger import ConversationLogger
 from .models.text2text.api.openai_models import OpenAI
 from .models.text2text.api.anthropic import AnthropicModel
```

### Comparing `promptify-2.0.2/promptify/models/text2text/api/anthropic.py` & `promptify-2.0.3/promptify/models/text2text/api/anthropic.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/models/text2text/api/azure_openai.py` & `promptify-2.0.3/promptify/models/text2text/api/azure_openai.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/models/text2text/api/base_model.py` & `promptify-2.0.3/promptify/models/text2text/api/base_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/models/text2text/api/cohere.py` & `promptify-2.0.3/promptify/models/text2text/api/cohere.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/models/text2text/api/hub_model.py` & `promptify-2.0.3/promptify/models/text2text/api/hub_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/models/text2text/api/mock_model.py` & `promptify-2.0.3/promptify/models/text2text/api/mock_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/models/text2text/api/openai_models.py` & `promptify-2.0.3/promptify/models/text2text/api/openai_models.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/parser/parser.py` & `promptify-2.0.3/promptify/parser/parser.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/pipelines/__init__.py` & `promptify-2.0.3/promptify/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompter/conversation_logger.py` & `promptify-2.0.3/promptify/prompter/conversation_logger.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompter/nlp_prompter.py` & `promptify-2.0.3/promptify/prompter/nlp_prompter.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompter/prompt_cache.py` & `promptify-2.0.3/promptify/prompter/prompt_cache.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompter/template_loader.py` & `promptify-2.0.3/promptify/prompter/template_loader.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/binary_classification/binary_classification.jinja` & `promptify-2.0.3/promptify/prompts/text2text/binary_classification/binary_classification.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/binary_classification/metadata.json` & `promptify-2.0.3/promptify/prompts/text2text/binary_classification/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/explain/explain.jinja` & `promptify-2.0.3/promptify/prompts/text2text/explain/explain.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/explain/metadata.json` & `promptify-2.0.3/promptify/prompts/text2text/explain/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/multiclass_classification/metadata.json` & `promptify-2.0.3/promptify/prompts/text2text/multiclass_classification/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/multiclass_classification/multiclass_classification.jinja` & `promptify-2.0.3/promptify/prompts/text2text/multiclass_classification/multiclass_classification.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/multiclass_classification/multiclass_gpt.jinja` & `promptify-2.0.3/promptify/prompts/text2text/multiclass_classification/multiclass_gpt.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/multilabel_classification/metadata.json` & `promptify-2.0.3/promptify/prompts/text2text/multilabel_classification/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/multilabel_classification/multilabel_classification.jinja` & `promptify-2.0.3/promptify/prompts/text2text/multilabel_classification/multilabel_classification.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/ner/metadata.json` & `promptify-2.0.3/promptify/prompts/text2text/ner/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/ner/ner_openai.jinja` & `promptify-2.0.3/promptify/prompts/text2text/ner/ner_openai.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/qa/qa.jinja` & `promptify-2.0.3/promptify/prompts/text2text/qa/qa.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/qa_gen/qa_gen.jinja` & `promptify-2.0.3/promptify/prompts/text2text/qa_gen/qa_gen.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/relation_extraction/metadata.json` & `promptify-2.0.3/promptify/prompts/text2text/relation_extraction/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/relation_extraction/relation_extraction.jinja` & `promptify-2.0.3/promptify/prompts/text2text/relation_extraction/relation_extraction.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/sql_writer/metadata.json` & `promptify-2.0.3/promptify/prompts/text2text/sql_writer/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/sql_writer/sql_writer_gpt.jinja` & `promptify-2.0.3/promptify/prompts/text2text/sql_writer/sql_writer_gpt.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/summary/summary.jinja` & `promptify-2.0.3/promptify/prompts/text2text/summary/summary.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/tabular_extractor/metadata.json` & `promptify-2.0.3/promptify/prompts/text2text/tabular_extractor/metadata.json`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/text_normalization/text_normalization_draft.jinja` & `promptify-2.0.3/promptify/prompts/text2text/text_normalization/text_normalization_draft.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/prompts/text2text/topic_modelling/topic_modeling_draft.jinja` & `promptify-2.0.3/promptify/prompts/text2text/topic_modelling/topic_modeling_draft.jinja`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/utils/conversation_utils.py` & `promptify-2.0.3/promptify/utils/conversation_utils.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/utils/data_utils.py` & `promptify-2.0.3/promptify/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify/utils/file_utils.py` & `promptify-2.0.3/promptify/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/promptify.egg-info/PKG-INFO` & `promptify-2.0.3/promptify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptify
-Version: 2.0.2
+Version: 2.0.3
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

 * *File "/tmp/diffoscope_psgtamyl_/tmpiv4uj_o1_TarContainer/0/115", line 109, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_psgtamyl_/tmpiv4uj_o1_TarContainer/0/115", line 109, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptify Version: 2.0.2 Summary: Use GPT or other
+Metadata-Version: 2.1 Name: promptify Version: 2.0.3 Summary: Use GPT or other
 prompt based models to get structured output Home-page: https://github.com/
 promptslab/Promptify Author: monk1337 Maintainer: The promptslab team with the
 help of all our contributors License: Apache Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE
  [https://raw.githubusercontent.com/promptslab/Promptify/main/assets/logo.png]
                             ****** Promptify ******
```

### Comparing `promptify-2.0.2/promptify.egg-info/SOURCES.txt` & `promptify-2.0.3/promptify.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements-dev.txt
+requirements.txt
 setup.py
 benchmarks/__init__.py
 examples/__init__.py
 examples/medical_ner.py
 promptify/VERSION
 promptify/__init__.py
 promptify.egg-info/PKG-INFO
```

### Comparing `promptify-2.0.2/setup.py` & `promptify-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/tests/unit_tests/models/test_base_model.py` & `promptify-2.0.3/tests/unit_tests/models/test_base_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/tests/unit_tests/models/test_hf_model.py` & `promptify-2.0.3/tests/unit_tests/models/test_hf_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/tests/unit_tests/models/test_openai_model.py` & `promptify-2.0.3/tests/unit_tests/models/test_openai_model.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/tests/unit_tests/parser/test_parser.py` & `promptify-2.0.3/tests/unit_tests/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `promptify-2.0.2/tests/unit_tests/prompter/test_prompter.py` & `promptify-2.0.3/tests/unit_tests/prompter/test_prompter.py`

 * *Files identical despite different names*


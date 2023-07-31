# Comparing `tmp/sapientml-0.1.2.tar.gz` & `tmp/sapientml-0.1.2.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapientml-0.1.2.tar", max compression
+gzip compressed data, was "sapientml-0.1.2.post0.tar", max compression
```

## Comparing `sapientml-0.1.2.tar` & `sapientml-0.1.2.post0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11351 2023-07-31 07:31:51.577479 sapientml-0.1.2/LICENSE
--rw-r--r--   0        0        0      903 2023-07-31 07:31:51.577479 sapientml-0.1.2/README.md
--rw-r--r--   0        0        0     2000 2023-07-31 07:32:09.721425 sapientml-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      639 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/__init__.py
--rw-r--r--   0        0        0      585 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/load/__init__.py
--rw-r--r--   0        0        0     2661 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/load/generator.py
--rw-r--r--   0        0        0      585 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/__init__.py
--rw-r--r--   0        0        0      585 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/__init__.py
--rw-r--r--   0        0        0     2248 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/artifacts/label_order.json
--rw-r--r--   0        0        0      585 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/generation/__init__.py
--rw-r--r--   0        0        0    27030 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/generation/pipeline_template.py
--rw-r--r--   0        0        0     1781 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/generation/predicate.py
--rw-r--r--   0        0        0     4592 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/generation/preprocessing_label.py
--rw-r--r--   0        0        0    16292 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/generation/template_based_adaptation.py
--rw-r--r--   0        0        0        0 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/design/__init__.py
--rw-r--r--   0        0        0     2831 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/design/label_util.py
--rw-r--r--   0        0        0     2761 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/design/pp_component_groups.py
--rw-r--r--   0        0        0     2194 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/design/search_space.py
--rw-r--r--   0        0        0      899 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/enums.py
--rw-r--r--   0        0        0     2514 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/generator.py
--rw-r--r--   0        0        0    37472 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/meta_features.py
--rw-r--r--   0        0        0    23684 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/models/feature_importance.json
--rw-r--r--   0        0        0     5658 2023-07-31 07:31:51.577479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/models/mp_model_1.pkl
--rw-r--r--   0        0        0   215382 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/models/mp_model_2.pkl
--rw-r--r--   0        0        0    12041 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/models/pp_models.pkl
--rw-r--r--   0        0        0     8478 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/params.py
--rw-r--r--   0        0        0     1975 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/ps_macros.py
--rw-r--r--   0        0        0      585 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/seeding/__init__.py
--rw-r--r--   0        0        0     8630 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/code_block_generator/prediction_based/seeding/predictor.py
--rw-r--r--   0        0        0        0 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/code_block_generator/rule_based/__init__.py
--rw-r--r--   0        0        0    10062 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/code_block_generator/rule_based/generator.py
--rw-r--r--   0        0        0     4370 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/executor.py
--rw-r--r--   0        0        0     3523 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/macros.py
--rw-r--r--   0        0        0    22810 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/main.py
--rw-r--r--   0        0        0    17853 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/params.py
--rw-r--r--   0        0        0    10236 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/result.py
--rw-r--r--   0        0        0     2067 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/suggestion.py
--rw-r--r--   0        0        0      585 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/util/__init__.py
--rw-r--r--   0        0        0     1570 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/util/json_util.py
--rw-r--r--   0        0        0      946 2023-07-31 07:31:51.581479 sapientml-0.1.2/sapientml/util/logging.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 sapientml-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-07-31 07:34:29.496246 sapientml-0.1.2.post0/LICENSE
+-rw-r--r--   0        0        0      864 2023-07-31 07:34:29.496246 sapientml-0.1.2.post0/README.md
+-rw-r--r--   0        0        0     2018 2023-07-31 07:34:47.436191 sapientml-0.1.2.post0/pyproject.toml
+-rw-r--r--   0        0        0      639 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/__init__.py
+-rw-r--r--   0        0        0      585 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/load/__init__.py
+-rw-r--r--   0        0        0     2661 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/load/generator.py
+-rw-r--r--   0        0        0      585 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/__init__.py
+-rw-r--r--   0        0        0      585 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/__init__.py
+-rw-r--r--   0        0        0     2248 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/artifacts/label_order.json
+-rw-r--r--   0        0        0      585 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/generation/__init__.py
+-rw-r--r--   0        0        0    27030 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/generation/pipeline_template.py
+-rw-r--r--   0        0        0     1781 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/generation/predicate.py
+-rw-r--r--   0        0        0     4592 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/generation/preprocessing_label.py
+-rw-r--r--   0        0        0    16292 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/generation/template_based_adaptation.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/design/__init__.py
+-rw-r--r--   0        0        0     2831 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/design/label_util.py
+-rw-r--r--   0        0        0     2761 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/design/pp_component_groups.py
+-rw-r--r--   0        0        0     2194 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/design/search_space.py
+-rw-r--r--   0        0        0      899 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/enums.py
+-rw-r--r--   0        0        0     2514 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/generator.py
+-rw-r--r--   0        0        0    37472 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/meta_features.py
+-rw-r--r--   0        0        0    23684 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/models/feature_importance.json
+-rw-r--r--   0        0        0     5658 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/models/mp_model_1.pkl
+-rw-r--r--   0        0        0   215382 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/models/mp_model_2.pkl
+-rw-r--r--   0        0        0    12041 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/models/pp_models.pkl
+-rw-r--r--   0        0        0     8478 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/params.py
+-rw-r--r--   0        0        0     1975 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/ps_macros.py
+-rw-r--r--   0        0        0      585 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/seeding/__init__.py
+-rw-r--r--   0        0        0     8630 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/seeding/predictor.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/rule_based/__init__.py
+-rw-r--r--   0        0        0    10062 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/code_block_generator/rule_based/generator.py
+-rw-r--r--   0        0        0     4370 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/executor.py
+-rw-r--r--   0        0        0     3523 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/macros.py
+-rw-r--r--   0        0        0    22810 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/main.py
+-rw-r--r--   0        0        0    17853 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/params.py
+-rw-r--r--   0        0        0    10236 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/result.py
+-rw-r--r--   0        0        0     2067 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/suggestion.py
+-rw-r--r--   0        0        0      585 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/util/__init__.py
+-rw-r--r--   0        0        0     1570 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/util/json_util.py
+-rw-r--r--   0        0        0      946 2023-07-31 07:34:29.500246 sapientml-0.1.2.post0/sapientml/util/logging.py
+-rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 sapientml-0.1.2.post0/PKG-INFO
```

### Comparing `sapientml-0.1.2/LICENSE` & `sapientml-0.1.2.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/README.md` & `sapientml-0.1.2.post0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # SapientML
 
-## Generative AutoML for Tabular Data
-
 # Getting Started
 ## Prerequisites
 
 - Python >=3.9,<3.11
 
 ## Installation
```

### Comparing `sapientml-0.1.2/pyproject.toml` & `sapientml-0.1.2.post0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sapientml"
-version = "0.1.2"
+version = "0.1.2.post0"
 description = "Generative AutoML for Tabular Data"
 authors = ["The SapientML Authors"]
 maintainers = [
     "Kosaku Kimura <kimura.kosaku@fujitsu.com>",
     "Akira Ura <ura.akira@fujitsu.com>",
 ]
 license = "Apache-2.0"
@@ -59,26 +59,26 @@
 pysen = "^0.10.5"
 pre-commit = "^3.3.3"
 jedi = "^0.19.0"
 pygount = "^1.6.1"
 tabulate = "^0.9.0"
 
 [tool.pysen]
-version = "0.1.2"
+version = "0.1.2.post0"
 
 [tool.pysen-cli]
 settings_dir = ".pysen"
 
 [tool.pysen.lint]
 enable_black = true
 enable_flake8 = true
 enable_isort = true
 enable_mypy = false
 line_length = 120
-py_version = "0.1.2"
+py_version = "0.1.2.post0"
 
 [tool.pysen.lint.source]
 includes = [
     "sapientml/", 
     "tests/", 
 ]
 [pytest]
```

### Comparing `sapientml-0.1.2/sapientml/__init__.py` & `sapientml-0.1.2.post0/sapientml/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/load/__init__.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/load/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/load/generator.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/load/generator.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/__init__.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/__init__.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/artifacts/label_order.json` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/artifacts/label_order.json`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/generation/__init__.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/generation/pipeline_template.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/generation/pipeline_template.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/generation/predicate.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/generation/predicate.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/generation/preprocessing_label.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/generation/preprocessing_label.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/adaptation/generation/template_based_adaptation.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/adaptation/generation/template_based_adaptation.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/design/label_util.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/design/label_util.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/design/pp_component_groups.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/design/pp_component_groups.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/design/search_space.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/design/search_space.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/enums.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/enums.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/generator.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/generator.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/meta_features.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/meta_features.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/models/feature_importance.json` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/models/feature_importance.json`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/models/mp_model_1.pkl` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/models/mp_model_1.pkl`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/models/mp_model_2.pkl` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/models/mp_model_2.pkl`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/models/pp_models.pkl` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/models/pp_models.pkl`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/params.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/params.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/ps_macros.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/ps_macros.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/seeding/__init__.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/seeding/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/prediction_based/seeding/predictor.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/prediction_based/seeding/predictor.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/code_block_generator/rule_based/generator.py` & `sapientml-0.1.2.post0/sapientml/code_block_generator/rule_based/generator.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/executor.py` & `sapientml-0.1.2.post0/sapientml/executor.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/macros.py` & `sapientml-0.1.2.post0/sapientml/macros.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/main.py` & `sapientml-0.1.2.post0/sapientml/main.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/params.py` & `sapientml-0.1.2.post0/sapientml/params.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/result.py` & `sapientml-0.1.2.post0/sapientml/result.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/suggestion.py` & `sapientml-0.1.2.post0/sapientml/suggestion.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/util/__init__.py` & `sapientml-0.1.2.post0/sapientml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/util/json_util.py` & `sapientml-0.1.2.post0/sapientml/util/json_util.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/sapientml/util/logging.py` & `sapientml-0.1.2.post0/sapientml/util/logging.py`

 * *Files identical despite different names*

### Comparing `sapientml-0.1.2/PKG-INFO` & `sapientml-0.1.2.post0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapientml
-Version: 0.1.2
+Version: 0.1.2.post0
 Summary: Generative AutoML for Tabular Data
 Home-page: https://github.com/sapientml/sapientml
 License: Apache-2.0
 Keywords: automl
 Author: The SapientML Authors
 Maintainer: Kosaku Kimura
 Maintainer-email: kimura.kosaku@fujitsu.com
@@ -30,16 +30,14 @@
 Requires-Dist: shap (>=0.42.1,<0.43.0)
 Requires-Dist: xgboost (>=1.7.6,<2.0.0)
 Project-URL: Repository, https://github.com/sapientml/sapientml
 Description-Content-Type: text/markdown
 
 # SapientML
 
-## Generative AutoML for Tabular Data
-
 # Getting Started
 ## Prerequisites
 
 - Python >=3.9,<3.11
 
 ## Installation
```


# Comparing `tmp/maud-metabolic-models-0.6.0.0.tar.gz` & `tmp/maud-metabolic-models-0.6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maud-metabolic-models-0.6.0.0.tar", last modified: Sun Jul 23 23:40:33 2023, max compression
+gzip compressed data, was "maud-metabolic-models-0.6.0.1.tar", last modified: Mon Jul 31 12:29:38 2023, max compression
```

## Comparing `maud-metabolic-models-0.6.0.0.tar` & `maud-metabolic-models-0.6.0.1.tar`

### file list

```diff
@@ -1,70 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.395416 maud-metabolic-models-0.6.0.0/maud/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.395416 maud-metabolic-models-0.6.0.0/maud/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.395416 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.399416 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/experimental_setup.toml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/inits.json
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/input_data_train.json
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.399416 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/expected_stan_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.395416 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.395416 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.399416 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/maud/data_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/hardcoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/id_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/kinetic_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/maud_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/maud_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/maud_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/maud_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/prior_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/getting_idatas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/getting_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/getting_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/getting_stan_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/loading_maud_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/parsing_kinetic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/running_stan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/maud/stan/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/stan/debug.stan
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/stan/functions.stan
--rw-r--r--   0 runner    (1001) docker     (123)    19181 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/stan/model.stan
--rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/stan/out_of_sample_model.stan
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.207764 maud-metabolic-models-0.6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-31 12:29:38.207764 maud-metabolic-models-0.6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.203764 maud-metabolic-models-0.6.0.1/maud/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.203764 maud-metabolic-models-0.6.0.1/maud/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.199764 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.203764 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/experimental_setup.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/inits.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/input_data_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.203764 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/expected_stan_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.203764 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/methionine/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/methionine/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/methionine/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/methionine/inits.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/methionine/methionine_cycle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/methionine/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    36103 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_inputs/methionine/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.199764 maud-metabolic-models-0.6.0.1/maud/data/example_outputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.199764 maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.207764 maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/user_input/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/user_input/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/user_input/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/user_input/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/user_input/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/user_input/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.207764 maud-metabolic-models-0.6.0.1/maud/data_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/hardcoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/id_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/kinetic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/maud_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/maud_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/maud_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/maud_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/data_model/prior_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/getting_idatas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/getting_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/getting_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/getting_stan_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/loading_maud_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/parsing_kinetic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/running_stan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.207764 maud-metabolic-models-0.6.0.1/maud/stan/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/stan/debug.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/stan/functions.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    19181 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/stan/model.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/stan/out_of_sample_model.stan
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/maud/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:38.207764 maud-metabolic-models-0.6.0.1/maud_metabolic_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-31 12:29:38.000000 maud-metabolic-models-0.6.0.1/maud_metabolic_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-31 12:29:38.000000 maud-metabolic-models-0.6.0.1/maud_metabolic_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:29:38.000000 maud-metabolic-models-0.6.0.1/maud_metabolic_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:29:38.000000 maud-metabolic-models-0.6.0.1/maud_metabolic_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-31 12:29:38.000000 maud-metabolic-models-0.6.0.1/maud_metabolic_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 12:29:38.000000 maud-metabolic-models-0.6.0.1/maud_metabolic_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:29:38.207764 maud-metabolic-models-0.6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-31 12:29:21.000000 maud-metabolic-models-0.6.0.1/setup.py
```

### Comparing `maud-metabolic-models-0.6.0.0/LICENSE` & `maud-metabolic-models-0.6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/PKG-INFO` & `maud-metabolic-models-0.6.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maud-metabolic-models
-Version: 0.6.0.0
+Version: 0.6.0.1
 Summary: Bayesian statistical models of metabolic networks
 Author: Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 License: GNU General Public License version 3
 Project-URL: homepage, https://github.com/biosustain/Maud
 Project-URL: download, https://pypi.org/project/maud-metabolic-models/
 Project-URL: documentation, https://maud-metabolic-models.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `maud-metabolic-models-0.6.0.0/README.rst` & `maud-metabolic-models-0.6.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/__init__.py` & `maud-metabolic-models-0.6.0.1/maud/__init__.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/analysis.py` & `maud-metabolic-models-0.6.0.1/maud/analysis.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/cli.py` & `maud-metabolic-models-0.6.0.1/maud/cli.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/experiments.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/inits.json` & `maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/inits.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/input_data_train.json` & `maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/input_data_train.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/kinetic_model.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/priors.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_inputs/example_ode/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/expected_stan_input.json` & `maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/expected_stan_input.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/experiments.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/kinetic_model.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/parameters.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/priors.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_inputs/linear/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/experiments.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/user_input/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/kinetic_model.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/user_input/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/parameters.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/user_input/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/priors.toml` & `maud-metabolic-models-0.6.0.1/maud/data/example_outputs/linear/user_input/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data_model/experiment.py` & `maud-metabolic-models-0.6.0.1/maud/data_model/experiment.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data_model/kinetic_model.py` & `maud-metabolic-models-0.6.0.1/maud/data_model/kinetic_model.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data_model/maud_config.py` & `maud-metabolic-models-0.6.0.1/maud/data_model/maud_config.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data_model/maud_init.py` & `maud-metabolic-models-0.6.0.1/maud/data_model/maud_init.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data_model/maud_input.py` & `maud-metabolic-models-0.6.0.1/maud/data_model/maud_input.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data_model/maud_parameter.py` & `maud-metabolic-models-0.6.0.1/maud/data_model/maud_parameter.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data_model/parameter_input.py` & `maud-metabolic-models-0.6.0.1/maud/data_model/parameter_input.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data_model/prior.py` & `maud-metabolic-models-0.6.0.1/maud/data_model/prior.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/data_model/prior_input.py` & `maud-metabolic-models-0.6.0.1/maud/data_model/prior_input.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/getting_idatas.py` & `maud-metabolic-models-0.6.0.1/maud/getting_idatas.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/getting_parameters.py` & `maud-metabolic-models-0.6.0.1/maud/getting_parameters.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/getting_priors.py` & `maud-metabolic-models-0.6.0.1/maud/getting_priors.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/getting_stan_inputs.py` & `maud-metabolic-models-0.6.0.1/maud/getting_stan_inputs.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/loading_maud_inputs.py` & `maud-metabolic-models-0.6.0.1/maud/loading_maud_inputs.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/parsing_kinetic_models.py` & `maud-metabolic-models-0.6.0.1/maud/parsing_kinetic_models.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/running_stan.py` & `maud-metabolic-models-0.6.0.1/maud/running_stan.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/stan/functions.stan` & `maud-metabolic-models-0.6.0.1/maud/stan/functions.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/stan/model.stan` & `maud-metabolic-models-0.6.0.1/maud/stan/model.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/stan/out_of_sample_model.stan` & `maud-metabolic-models-0.6.0.1/maud/stan/out_of_sample_model.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud/utility_functions.py` & `maud-metabolic-models-0.6.0.1/maud/utility_functions.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/PKG-INFO` & `maud-metabolic-models-0.6.0.1/maud_metabolic_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maud-metabolic-models
-Version: 0.6.0.0
+Version: 0.6.0.1
 Summary: Bayesian statistical models of metabolic networks
 Author: Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 License: GNU General Public License version 3
 Project-URL: homepage, https://github.com/biosustain/Maud
 Project-URL: download, https://pypi.org/project/maud-metabolic-models/
 Project-URL: documentation, https://maud-metabolic-models.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/SOURCES.txt` & `maud-metabolic-models-0.6.0.1/maud_metabolic_models.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 maud/data/example_inputs/example_ode/priors.toml
 maud/data/example_inputs/linear/config.toml
 maud/data/example_inputs/linear/expected_stan_input.json
 maud/data/example_inputs/linear/experiments.toml
 maud/data/example_inputs/linear/kinetic_model.toml
 maud/data/example_inputs/linear/parameters.toml
 maud/data/example_inputs/linear/priors.toml
+maud/data/example_inputs/methionine/config.toml
+maud/data/example_inputs/methionine/experiments.toml
+maud/data/example_inputs/methionine/inits.toml
+maud/data/example_inputs/methionine/methionine_cycle.toml
+maud/data/example_inputs/methionine/parameters.toml
+maud/data/example_inputs/methionine/priors.toml
 maud/data/example_outputs/linear/user_input/config.toml
 maud/data/example_outputs/linear/user_input/experiments.toml
 maud/data/example_outputs/linear/user_input/kinetic_model.toml
 maud/data/example_outputs/linear/user_input/parameters.toml
 maud/data/example_outputs/linear/user_input/priors.toml
 maud/data_model/__init__.py
 maud/data_model/experiment.py
```

### Comparing `maud-metabolic-models-0.6.0.0/pyproject.toml` & `maud-metabolic-models-0.6.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "cmdstanpy >= 1.0.7", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maud-metabolic-models"
-version = "0.6.0.0"
+version = "0.6.0.1"
 authors = [
     {name = "Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark"}
   ]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -69,16 +69,17 @@
     "maud",
     "maud.data_model",
     # non-python code packages
     "maud.stan",
     # data packages
     "maud.data",
     "maud.data.example_inputs",
-    "maud.data.example_inputs.linear",
     "maud.data.example_inputs.example_ode",
+    "maud.data.example_inputs.linear",
+    "maud.data.example_inputs.methionine",
     "maud.data.example_outputs",
     "maud.data.example_outputs.linear",
     "maud.data.example_outputs.linear.user_input",
 ]
 [tool.setuptools.package-data]
 "*" = ["*.stan", "*.json", "*.toml"]
```

### Comparing `maud-metabolic-models-0.6.0.0/setup.py` & `maud-metabolic-models-0.6.0.1/setup.py`

 * *Files identical despite different names*


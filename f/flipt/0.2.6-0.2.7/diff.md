# Comparing `tmp/flipt-0.2.6.tar.gz` & `tmp/flipt-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipt-0.2.6.tar", max compression
+gzip compressed data, was "flipt-0.2.7.tar", max compression
```

## Comparing `flipt-0.2.6.tar` & `flipt-0.2.7.tar`

### file list

```diff
@@ -1,90 +1,115 @@
--rw-r--r--   0        0        0     1077 2023-06-22 18:40:07.522438 flipt-0.2.6/LICENSE
--rw-r--r--   0        0        0     1354 2023-06-22 18:40:07.522438 flipt-0.2.6/README.md
--rw-r--r--   0        0        0      365 2023-06-22 18:40:07.522438 flipt-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2491 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/__init__.py
--rw-r--r--   0        0        0     3836 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/client.py
--rw-r--r--   0        0        0      348 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      158 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/environment.py
--rw-r--r--   0        0        0        0 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/py.typed
--rw-r--r--   0        0        0     2513 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/__init__.py
--rw-r--r--   0        0        0      261 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/__init__.py
--rw-r--r--   0        0        0     9429 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/client.py
--rw-r--r--   0        0        0      369 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/types/__init__.py
--rw-r--r--   0        0        0     1128 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/types/authentication.py
--rw-r--r--   0        0        0      943 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/types/authentication_list.py
--rw-r--r--   0        0        0      988 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/types/authentication_method.py
--rw-r--r--   0        0        0      925 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/types/authentication_token.py
--rw-r--r--   0        0        0       65 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth_method_k_8_s/__init__.py
--rw-r--r--   0        0        0     2889 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth_method_k_8_s/client.py
--rw-r--r--   0        0        0      195 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_oidc/__init__.py
--rw-r--r--   0        0        0     4699 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_oidc/client.py
--rw-r--r--   0        0        0      252 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_oidc/types/__init__.py
--rw-r--r--   0        0        0      854 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py
--rw-r--r--   0        0        0      833 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py
--rw-r--r--   0        0        0       65 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_token/__init__.py
--rw-r--r--   0        0        0     3352 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_token/client.py
--rw-r--r--   0        0        0      117 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/commons/__init__.py
--rw-r--r--   0        0        0      120 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/commons/types/__init__.py
--rw-r--r--   0        0        0      933 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/commons/types/pageable.py
--rw-r--r--   0        0        0      279 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/__init__.py
--rw-r--r--   0        0        0     6805 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/client.py
--rw-r--r--   0        0        0      399 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/types/__init__.py
--rw-r--r--   0        0        0     1148 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/types/constraint.py
--rw-r--r--   0        0        0     1454 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/types/constraint_comparison_type.py
--rw-r--r--   0        0        0      951 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/types/constraint_create_request.py
--rw-r--r--   0        0        0      951 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/types/constraint_update_request.py
--rw-r--r--   0        0        0      237 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/__init__.py
--rw-r--r--   0        0        0     7340 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/client.py
--rw-r--r--   0        0        0      324 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/types/__init__.py
--rw-r--r--   0        0        0     1045 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/types/distribution.py
--rw-r--r--   0        0        0      868 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/types/distribution_create_request.py
--rw-r--r--   0        0        0      868 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/types/distribution_update_request.py
--rw-r--r--   0        0        0      365 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/__init__.py
--rw-r--r--   0        0        0     4982 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/client.py
--rw-r--r--   0        0        0      490 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/__init__.py
--rw-r--r--   0        0        0     1045 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/batch_evaluation_request.py
--rw-r--r--   0        0        0     1029 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/batch_evaluation_response.py
--rw-r--r--   0        0        0     1446 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_reason.py
--rw-r--r--   0        0        0      999 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_request.py
--rw-r--r--   0        0        0     1328 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_response.py
--rw-r--r--   0        0        0      211 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/__init__.py
--rw-r--r--   0        0        0    10180 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/client.py
--rw-r--r--   0        0        0      296 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/types/__init__.py
--rw-r--r--   0        0        0     1047 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/types/flag.py
--rw-r--r--   0        0        0      839 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/types/flag_create_request.py
--rw-r--r--   0        0        0      951 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/types/flag_list.py
--rw-r--r--   0        0        0      826 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/types/flag_update_request.py
--rw-r--r--   0        0        0      251 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/__init__.py
--rw-r--r--   0        0        0     9890 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/client.py
--rw-r--r--   0        0        0      356 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/types/__init__.py
--rw-r--r--   0        0        0      973 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/types/namespace.py
--rw-r--r--   0        0        0      809 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_create_request.py
--rw-r--r--   0        0        0      976 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_list.py
--rw-r--r--   0        0        0      796 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_update_request.py
--rw-r--r--   0        0        0      249 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/__init__.py
--rw-r--r--   0        0        0    12614 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/client.py
--rw-r--r--   0        0        0      365 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1142 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/rule.py
--rw-r--r--   0        0        0      857 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/rule_create_request.py
--rw-r--r--   0        0        0      951 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/rule_list.py
--rw-r--r--   0        0        0      849 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/rule_order_request.py
--rw-r--r--   0        0        0      843 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/rule_update_request.py
--rw-r--r--   0        0        0      273 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/__init__.py
--rw-r--r--   0        0        0    10414 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/client.py
--rw-r--r--   0        0        0      401 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/__init__.py
--rw-r--r--   0        0        0     1165 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/segment.py
--rw-r--r--   0        0        0      954 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/segment_create_request.py
--rw-r--r--   0        0        0      966 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/segment_list.py
--rw-r--r--   0        0        0      566 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/segment_match_type.py
--rw-r--r--   0        0        0      941 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/segment_update_request.py
--rw-r--r--   0        0        0      207 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/__init__.py
--rw-r--r--   0        0        0     6724 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/client.py
--rw-r--r--   0        0        0      279 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/types/__init__.py
--rw-r--r--   0        0        0     1035 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/types/variant.py
--rw-r--r--   0        0        0      861 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/types/variant_create_request.py
--rw-r--r--   0        0        0      861 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/types/variant_update_request.py
--rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 flipt-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-31 14:25:47.502846 flipt-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1354 2023-07-31 14:25:47.502846 flipt-0.2.7/README.md
+-rw-r--r--   0        0        0      365 2023-07-31 14:25:47.502846 flipt-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2933 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/__init__.py
+-rw-r--r--   0        0        0     4366 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/client.py
+-rw-r--r--   0        0        0      348 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      158 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/environment.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/py.typed
+-rw-r--r--   0        0        0     2977 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/__init__.py
+-rw-r--r--   0        0        0      261 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth/__init__.py
+-rw-r--r--   0        0        0     9429 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth/client.py
+-rw-r--r--   0        0        0      369 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth/types/__init__.py
+-rw-r--r--   0        0        0     1128 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth/types/authentication.py
+-rw-r--r--   0        0        0      943 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth/types/authentication_list.py
+-rw-r--r--   0        0        0      988 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth/types/authentication_method.py
+-rw-r--r--   0        0        0      925 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth/types/authentication_token.py
+-rw-r--r--   0        0        0       65 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth_method_k_8_s/__init__.py
+-rw-r--r--   0        0        0     2889 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth_method_k_8_s/client.py
+-rw-r--r--   0        0        0      195 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth_method_oidc/__init__.py
+-rw-r--r--   0        0        0     4699 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth_method_oidc/client.py
+-rw-r--r--   0        0        0      252 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth_method_oidc/types/__init__.py
+-rw-r--r--   0        0        0      854 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py
+-rw-r--r--   0        0        0      833 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py
+-rw-r--r--   0        0        0       65 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth_method_token/__init__.py
+-rw-r--r--   0        0        0     3352 2023-07-31 14:25:47.502846 flipt-0.2.7/src/flipt/resources/auth_method_token/client.py
+-rw-r--r--   0        0        0      117 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/commons/__init__.py
+-rw-r--r--   0        0        0      120 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0      933 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/commons/types/pageable.py
+-rw-r--r--   0        0        0      279 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/constraints/__init__.py
+-rw-r--r--   0        0        0     6805 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/constraints/client.py
+-rw-r--r--   0        0        0      399 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/constraints/types/__init__.py
+-rw-r--r--   0        0        0     1210 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/constraints/types/constraint.py
+-rw-r--r--   0        0        0     1454 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/constraints/types/constraint_comparison_type.py
+-rw-r--r--   0        0        0      951 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/constraints/types/constraint_create_request.py
+-rw-r--r--   0        0        0      951 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/constraints/types/constraint_update_request.py
+-rw-r--r--   0        0        0      237 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/distributions/__init__.py
+-rw-r--r--   0        0        0     7340 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/distributions/client.py
+-rw-r--r--   0        0        0      324 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/distributions/types/__init__.py
+-rw-r--r--   0        0        0     1045 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/distributions/types/distribution.py
+-rw-r--r--   0        0        0      868 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/distributions/types/distribution_create_request.py
+-rw-r--r--   0        0        0      868 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/distributions/types/distribution_update_request.py
+-rw-r--r--   0        0        0      365 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluate/__init__.py
+-rw-r--r--   0        0        0     4982 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluate/client.py
+-rw-r--r--   0        0        0      490 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluate/types/__init__.py
+-rw-r--r--   0        0        0     1045 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluate/types/batch_evaluation_request.py
+-rw-r--r--   0        0        0     1029 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluate/types/batch_evaluation_response.py
+-rw-r--r--   0        0        0     1446 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluate/types/evaluation_reason.py
+-rw-r--r--   0        0        0      999 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluate/types/evaluation_request.py
+-rw-r--r--   0        0        0     1328 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluate/types/evaluation_response.py
+-rw-r--r--   0        0        0      667 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/__init__.py
+-rw-r--r--   0        0        0     6681 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/client.py
+-rw-r--r--   0        0        0      963 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/__init__.py
+-rw-r--r--   0        0        0      958 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/batch_evaluation_request.py
+-rw-r--r--   0        0        0     1029 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/batch_evaluation_response.py
+-rw-r--r--   0        0        0     1054 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/boolean_evaluation_response.py
+-rw-r--r--   0        0        0      778 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/error_evaluation_reason.py
+-rw-r--r--   0        0        0      998 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/error_evaluation_response.py
+-rw-r--r--   0        0        0     1185 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/evaluation_reason.py
+-rw-r--r--   0        0        0     1061 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/evaluation_request.py
+-rw-r--r--   0        0        0     1222 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/evaluation_response.py
+-rw-r--r--   0        0        0     1048 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/evaluation_response_type.py
+-rw-r--r--   0        0        0     1255 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/evaluation/types/variant_evaluation_response.py
+-rw-r--r--   0        0        0      233 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/flags/__init__.py
+-rw-r--r--   0        0        0    10180 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/flags/client.py
+-rw-r--r--   0        0        0      340 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/flags/types/__init__.py
+-rw-r--r--   0        0        0     1160 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/flags/types/flag.py
+-rw-r--r--   0        0        0      890 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/flags/types/flag_create_request.py
+-rw-r--r--   0        0        0      951 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/flags/types/flag_list.py
+-rw-r--r--   0        0        0      572 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/flags/types/flag_type.py
+-rw-r--r--   0        0        0      826 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/flags/types/flag_update_request.py
+-rw-r--r--   0        0        0      251 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/namespaces/__init__.py
+-rw-r--r--   0        0        0     9890 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/namespaces/client.py
+-rw-r--r--   0        0        0      356 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/namespaces/types/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/namespaces/types/namespace.py
+-rw-r--r--   0        0        0      809 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/namespaces/types/namespace_create_request.py
+-rw-r--r--   0        0        0      976 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/namespaces/types/namespace_list.py
+-rw-r--r--   0        0        0      796 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/namespaces/types/namespace_update_request.py
+-rw-r--r--   0        0        0      451 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/__init__.py
+-rw-r--r--   0        0        0    12740 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/client.py
+-rw-r--r--   0        0        0      628 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/types/__init__.py
+-rw-r--r--   0        0        0     1310 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/types/rollout.py
+-rw-r--r--   0        0        0      980 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/types/rollout_create_request.py
+-rw-r--r--   0        0        0      966 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/types/rollout_list.py
+-rw-r--r--   0        0        0      858 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/types/rollout_order_request.py
+-rw-r--r--   0        0        0      856 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/types/rollout_segment.py
+-rw-r--r--   0        0        0      776 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/types/rollout_threshold.py
+-rw-r--r--   0        0        0      844 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/types/rollout_type.py
+-rw-r--r--   0        0        0      966 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rollouts/types/rollout_update_request.py
+-rw-r--r--   0        0        0      249 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rules/__init__.py
+-rw-r--r--   0        0        0    12614 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rules/client.py
+-rw-r--r--   0        0        0      365 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1204 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rules/types/rule.py
+-rw-r--r--   0        0        0      857 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rules/types/rule_create_request.py
+-rw-r--r--   0        0        0      951 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rules/types/rule_list.py
+-rw-r--r--   0        0        0      849 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rules/types/rule_order_request.py
+-rw-r--r--   0        0        0      843 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/rules/types/rule_update_request.py
+-rw-r--r--   0        0        0      273 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/segments/__init__.py
+-rw-r--r--   0        0        0    10414 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/segments/client.py
+-rw-r--r--   0        0        0      401 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/segments/types/__init__.py
+-rw-r--r--   0        0        0     1227 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/segments/types/segment.py
+-rw-r--r--   0        0        0      954 2023-07-31 14:25:47.506846 flipt-0.2.7/src/flipt/resources/segments/types/segment_create_request.py
+-rw-r--r--   0        0        0      966 2023-07-31 14:25:47.510846 flipt-0.2.7/src/flipt/resources/segments/types/segment_list.py
+-rw-r--r--   0        0        0      566 2023-07-31 14:25:47.510846 flipt-0.2.7/src/flipt/resources/segments/types/segment_match_type.py
+-rw-r--r--   0        0        0      941 2023-07-31 14:25:47.510846 flipt-0.2.7/src/flipt/resources/segments/types/segment_update_request.py
+-rw-r--r--   0        0        0      207 2023-07-31 14:25:47.510846 flipt-0.2.7/src/flipt/resources/variants/__init__.py
+-rw-r--r--   0        0        0     6724 2023-07-31 14:25:47.510846 flipt-0.2.7/src/flipt/resources/variants/client.py
+-rw-r--r--   0        0        0      279 2023-07-31 14:25:47.510846 flipt-0.2.7/src/flipt/resources/variants/types/__init__.py
+-rw-r--r--   0        0        0     1097 2023-07-31 14:25:47.510846 flipt-0.2.7/src/flipt/resources/variants/types/variant.py
+-rw-r--r--   0        0        0      861 2023-07-31 14:25:47.510846 flipt-0.2.7/src/flipt/resources/variants/types/variant_create_request.py
+-rw-r--r--   0        0        0      861 2023-07-31 14:25:47.510846 flipt-0.2.7/src/flipt/resources/variants/types/variant_update_request.py
+-rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 flipt-0.2.7/PKG-INFO
```

### Comparing `flipt-0.2.6/LICENSE` & `flipt-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/README.md` & `flipt-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/__init__.py` & `flipt-0.2.7/src/flipt/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,22 +17,31 @@
     DistributionUpdateRequest,
     EvaluationReason,
     EvaluationRequest,
     EvaluationResponse,
     Flag,
     FlagCreateRequest,
     FlagList,
+    FlagType,
     FlagUpdateRequest,
     Namespace,
     NamespaceCreateRequest,
     NamespaceList,
     NamespaceUpdateRequest,
     OidcAuthorizeUrlResponse,
     OidcCallbackResponse,
     Pageable,
+    Rollout,
+    RolloutCreateRequest,
+    RolloutList,
+    RolloutOrderRequest,
+    RolloutSegment,
+    RolloutThreshold,
+    RolloutType,
+    RolloutUpdateRequest,
     Rule,
     RuleCreateRequest,
     RuleList,
     RuleOrderRequest,
     RuleUpdateRequest,
     Segment,
     SegmentCreateRequest,
@@ -46,16 +55,18 @@
     auth_method_k_8_s,
     auth_method_oidc,
     auth_method_token,
     commons,
     constraints,
     distributions,
     evaluate,
+    evaluation,
     flags,
     namespaces,
+    rollouts,
     rules,
     segments,
     variants,
 )
 
 __all__ = [
     "Authentication",
@@ -73,23 +84,32 @@
     "DistributionUpdateRequest",
     "EvaluationReason",
     "EvaluationRequest",
     "EvaluationResponse",
     "Flag",
     "FlagCreateRequest",
     "FlagList",
+    "FlagType",
     "FlagUpdateRequest",
     "FliptApiEnvironment",
     "Namespace",
     "NamespaceCreateRequest",
     "NamespaceList",
     "NamespaceUpdateRequest",
     "OidcAuthorizeUrlResponse",
     "OidcCallbackResponse",
     "Pageable",
+    "Rollout",
+    "RolloutCreateRequest",
+    "RolloutList",
+    "RolloutOrderRequest",
+    "RolloutSegment",
+    "RolloutThreshold",
+    "RolloutType",
+    "RolloutUpdateRequest",
     "Rule",
     "RuleCreateRequest",
     "RuleList",
     "RuleOrderRequest",
     "RuleUpdateRequest",
     "Segment",
     "SegmentCreateRequest",
@@ -103,13 +123,15 @@
     "auth_method_k_8_s",
     "auth_method_oidc",
     "auth_method_token",
     "commons",
     "constraints",
     "distributions",
     "evaluate",
+    "evaluation",
     "flags",
     "namespaces",
+    "rollouts",
     "rules",
     "segments",
     "variants",
 ]
```

### Comparing `flipt-0.2.6/src/flipt/client.py` & `flipt-0.2.7/src/flipt/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,52 +6,58 @@
 from .resources.auth.client import AsyncAuthClient, AuthClient
 from .resources.auth_method_k_8_s.client import AsyncAuthMethodK8SClient, AuthMethodK8SClient
 from .resources.auth_method_oidc.client import AsyncAuthMethodOidcClient, AuthMethodOidcClient
 from .resources.auth_method_token.client import AsyncAuthMethodTokenClient, AuthMethodTokenClient
 from .resources.constraints.client import AsyncConstraintsClient, ConstraintsClient
 from .resources.distributions.client import AsyncDistributionsClient, DistributionsClient
 from .resources.evaluate.client import AsyncEvaluateClient, EvaluateClient
+from .resources.evaluation.client import AsyncEvaluationClient, EvaluationClient
 from .resources.flags.client import AsyncFlagsClient, FlagsClient
 from .resources.namespaces.client import AsyncNamespacesClient, NamespacesClient
+from .resources.rollouts.client import AsyncRolloutsClient, RolloutsClient
 from .resources.rules.client import AsyncRulesClient, RulesClient
 from .resources.segments.client import AsyncSegmentsClient, SegmentsClient
 from .resources.variants.client import AsyncVariantsClient, VariantsClient
 
 
 class FliptApi:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
+        self.evaluation = EvaluationClient(environment=self._environment, token=self._token)
         self.auth_method_k_8_s = AuthMethodK8SClient(environment=self._environment, token=self._token)
         self.auth_method_oidc = AuthMethodOidcClient(environment=self._environment, token=self._token)
         self.auth_method_token = AuthMethodTokenClient(environment=self._environment, token=self._token)
         self.auth = AuthClient(environment=self._environment, token=self._token)
         self.constraints = ConstraintsClient(environment=self._environment, token=self._token)
         self.distributions = DistributionsClient(environment=self._environment, token=self._token)
         self.evaluate = EvaluateClient(environment=self._environment, token=self._token)
         self.flags = FlagsClient(environment=self._environment, token=self._token)
         self.namespaces = NamespacesClient(environment=self._environment, token=self._token)
+        self.rollouts = RolloutsClient(environment=self._environment, token=self._token)
         self.rules = RulesClient(environment=self._environment, token=self._token)
         self.segments = SegmentsClient(environment=self._environment, token=self._token)
         self.variants = VariantsClient(environment=self._environment, token=self._token)
 
 
 class AsyncFliptApi:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
+        self.evaluation = AsyncEvaluationClient(environment=self._environment, token=self._token)
         self.auth_method_k_8_s = AsyncAuthMethodK8SClient(environment=self._environment, token=self._token)
         self.auth_method_oidc = AsyncAuthMethodOidcClient(environment=self._environment, token=self._token)
         self.auth_method_token = AsyncAuthMethodTokenClient(environment=self._environment, token=self._token)
         self.auth = AsyncAuthClient(environment=self._environment, token=self._token)
         self.constraints = AsyncConstraintsClient(environment=self._environment, token=self._token)
         self.distributions = AsyncDistributionsClient(environment=self._environment, token=self._token)
         self.evaluate = AsyncEvaluateClient(environment=self._environment, token=self._token)
         self.flags = AsyncFlagsClient(environment=self._environment, token=self._token)
         self.namespaces = AsyncNamespacesClient(environment=self._environment, token=self._token)
+        self.rollouts = AsyncRolloutsClient(environment=self._environment, token=self._token)
         self.rules = AsyncRulesClient(environment=self._environment, token=self._token)
         self.segments = AsyncSegmentsClient(environment=self._environment, token=self._token)
         self.variants = AsyncVariantsClient(environment=self._environment, token=self._token)
```

### Comparing `flipt-0.2.6/src/flipt/core/datetime_utils.py` & `flipt-0.2.7/src/flipt/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/core/jsonable_encoder.py` & `flipt-0.2.7/src/flipt/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/__init__.py` & `flipt-0.2.7/src/flipt/resources/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,18 @@
     auth_method_k_8_s,
     auth_method_oidc,
     auth_method_token,
     commons,
     constraints,
     distributions,
     evaluate,
+    evaluation,
     flags,
     namespaces,
+    rollouts,
     rules,
     segments,
     variants,
 )
 from .auth import Authentication, AuthenticationList, AuthenticationMethod, AuthenticationToken
 from .auth_method_oidc import OidcAuthorizeUrlResponse, OidcCallbackResponse
 from .commons import Pageable
@@ -23,16 +25,26 @@
 from .evaluate import (
     BatchEvaluationRequest,
     BatchEvaluationResponse,
     EvaluationReason,
     EvaluationRequest,
     EvaluationResponse,
 )
-from .flags import Flag, FlagCreateRequest, FlagList, FlagUpdateRequest
+from .flags import Flag, FlagCreateRequest, FlagList, FlagType, FlagUpdateRequest
 from .namespaces import Namespace, NamespaceCreateRequest, NamespaceList, NamespaceUpdateRequest
+from .rollouts import (
+    Rollout,
+    RolloutCreateRequest,
+    RolloutList,
+    RolloutOrderRequest,
+    RolloutSegment,
+    RolloutThreshold,
+    RolloutType,
+    RolloutUpdateRequest,
+)
 from .rules import Rule, RuleCreateRequest, RuleList, RuleOrderRequest, RuleUpdateRequest
 from .segments import Segment, SegmentCreateRequest, SegmentList, SegmentMatchType, SegmentUpdateRequest
 from .variants import Variant, VariantCreateRequest, VariantUpdateRequest
 
 __all__ = [
     "Authentication",
     "AuthenticationList",
@@ -49,22 +61,31 @@
     "DistributionUpdateRequest",
     "EvaluationReason",
     "EvaluationRequest",
     "EvaluationResponse",
     "Flag",
     "FlagCreateRequest",
     "FlagList",
+    "FlagType",
     "FlagUpdateRequest",
     "Namespace",
     "NamespaceCreateRequest",
     "NamespaceList",
     "NamespaceUpdateRequest",
     "OidcAuthorizeUrlResponse",
     "OidcCallbackResponse",
     "Pageable",
+    "Rollout",
+    "RolloutCreateRequest",
+    "RolloutList",
+    "RolloutOrderRequest",
+    "RolloutSegment",
+    "RolloutThreshold",
+    "RolloutType",
+    "RolloutUpdateRequest",
     "Rule",
     "RuleCreateRequest",
     "RuleList",
     "RuleOrderRequest",
     "RuleUpdateRequest",
     "Segment",
     "SegmentCreateRequest",
@@ -78,13 +99,15 @@
     "auth_method_k_8_s",
     "auth_method_oidc",
     "auth_method_token",
     "commons",
     "constraints",
     "distributions",
     "evaluate",
+    "evaluation",
     "flags",
     "namespaces",
+    "rollouts",
     "rules",
     "segments",
     "variants",
 ]
```

### Comparing `flipt-0.2.6/src/flipt/resources/auth/client.py` & `flipt-0.2.7/src/flipt/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/auth/types/authentication.py` & `flipt-0.2.7/src/flipt/resources/auth/types/authentication.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/auth/types/authentication_list.py` & `flipt-0.2.7/src/flipt/resources/auth/types/authentication_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/auth/types/authentication_method.py` & `flipt-0.2.7/src/flipt/resources/auth/types/authentication_method.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/auth/types/authentication_token.py` & `flipt-0.2.7/src/flipt/resources/auth/types/authentication_token.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/auth_method_k_8_s/client.py` & `flipt-0.2.7/src/flipt/resources/auth_method_k_8_s/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/auth_method_oidc/client.py` & `flipt-0.2.7/src/flipt/resources/auth_method_oidc/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py` & `flipt-0.2.7/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py` & `flipt-0.2.7/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/auth_method_token/client.py` & `flipt-0.2.7/src/flipt/resources/auth_method_token/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/commons/types/pageable.py` & `flipt-0.2.7/src/flipt/resources/commons/types/pageable.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/constraints/client.py` & `flipt-0.2.7/src/flipt/resources/constraints/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/constraints/types/constraint.py` & `flipt-0.2.7/src/flipt/resources/constraints/types/constraint.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from ....core.datetime_utils import serialize_datetime
 from .constraint_comparison_type import ConstraintComparisonType
 
 
 class Constraint(pydantic.BaseModel):
     id: str
+    namespace_key: str = pydantic.Field(alias="namespaceKey")
     segment_key: str = pydantic.Field(alias="segmentKey")
     type: ConstraintComparisonType
     property: str
     operator: str
     value: str
     description: str
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
```

### Comparing `flipt-0.2.6/src/flipt/resources/constraints/types/constraint_comparison_type.py` & `flipt-0.2.7/src/flipt/resources/constraints/types/constraint_comparison_type.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/constraints/types/constraint_create_request.py` & `flipt-0.2.7/src/flipt/resources/constraints/types/constraint_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/constraints/types/constraint_update_request.py` & `flipt-0.2.7/src/flipt/resources/constraints/types/constraint_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/distributions/client.py` & `flipt-0.2.7/src/flipt/resources/distributions/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/distributions/types/distribution.py` & `flipt-0.2.7/src/flipt/resources/distributions/types/distribution.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/distributions/types/distribution_create_request.py` & `flipt-0.2.7/src/flipt/resources/distributions/types/distribution_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/distributions/types/distribution_update_request.py` & `flipt-0.2.7/src/flipt/resources/distributions/types/distribution_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/evaluate/client.py` & `flipt-0.2.7/src/flipt/resources/evaluate/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/evaluate/types/batch_evaluation_request.py` & `flipt-0.2.7/src/flipt/resources/evaluate/types/batch_evaluation_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/evaluate/types/batch_evaluation_response.py` & `flipt-0.2.7/src/flipt/resources/evaluate/types/batch_evaluation_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_reason.py` & `flipt-0.2.7/src/flipt/resources/evaluate/types/evaluation_reason.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_request.py` & `flipt-0.2.7/src/flipt/resources/evaluate/types/evaluation_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_response.py` & `flipt-0.2.7/src/flipt/resources/evaluate/types/evaluation_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/flags/client.py` & `flipt-0.2.7/src/flipt/resources/flags/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/flags/types/flag.py` & `flipt-0.2.7/src/flipt/resources/flags/types/flag.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...variants.types.variant import Variant
+from .flag_type import FlagType
 
 
 class Flag(pydantic.BaseModel):
+    namespace_key: str = pydantic.Field(alias="namespaceKey")
     key: str
     name: str
     description: str
     enabled: bool
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
     variants: typing.List[Variant]
+    type: FlagType
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.6/src/flipt/resources/flags/types/flag_create_request.py` & `flipt-0.2.7/src/flipt/resources/namespaces/types/namespace_update_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class FlagCreateRequest(pydantic.BaseModel):
-    key: str
+class NamespaceUpdateRequest(pydantic.BaseModel):
     name: str
     description: typing.Optional[str]
-    enabled: typing.Optional[bool]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.6/src/flipt/resources/flags/types/flag_list.py` & `flipt-0.2.7/src/flipt/resources/flags/types/flag_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/flags/types/flag_update_request.py` & `flipt-0.2.7/src/flipt/resources/flags/types/flag_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/namespaces/client.py` & `flipt-0.2.7/src/flipt/resources/namespaces/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/namespaces/types/namespace.py` & `flipt-0.2.7/src/flipt/resources/namespaces/types/namespace.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_create_request.py` & `flipt-0.2.7/src/flipt/resources/namespaces/types/namespace_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_list.py` & `flipt-0.2.7/src/flipt/resources/namespaces/types/namespace_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_update_request.py` & `flipt-0.2.7/src/flipt/resources/variants/types/variant_update_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class NamespaceUpdateRequest(pydantic.BaseModel):
-    name: str
+class VariantUpdateRequest(pydantic.BaseModel):
+    key: str
+    name: typing.Optional[str]
     description: typing.Optional[str]
+    attachment: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.6/src/flipt/resources/rules/client.py` & `flipt-0.2.7/src/flipt/resources/rules/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/rules/types/rule.py` & `flipt-0.2.7/src/flipt/resources/variants/types/variant.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...distributions.types.distribution import Distribution
 
 
-class Rule(pydantic.BaseModel):
+class Variant(pydantic.BaseModel):
     id: str
+    namespace_key: str = pydantic.Field(alias="namespaceKey")
     flag_key: str = pydantic.Field(alias="flagKey")
-    segment_key: str = pydantic.Field(alias="segmentKey")
-    distributions: typing.List[Distribution]
-    rank: int
+    key: str
+    name: str
+    description: str
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+    attachment: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.6/src/flipt/resources/rules/types/rule_create_request.py` & `flipt-0.2.7/src/flipt/resources/rules/types/rule_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/rules/types/rule_list.py` & `flipt-0.2.7/src/flipt/resources/rules/types/rule_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/rules/types/rule_order_request.py` & `flipt-0.2.7/src/flipt/resources/rules/types/rule_order_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/rules/types/rule_update_request.py` & `flipt-0.2.7/src/flipt/resources/rules/types/rule_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/segments/client.py` & `flipt-0.2.7/src/flipt/resources/segments/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/segments/types/segment.py` & `flipt-0.2.7/src/flipt/resources/segments/types/segment.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from ....core.datetime_utils import serialize_datetime
 from ...constraints.types.constraint import Constraint
 from .segment_match_type import SegmentMatchType
 
 
 class Segment(pydantic.BaseModel):
+    namespace_key: str = pydantic.Field(alias="namespaceKey")
     key: str
     name: str
     description: str
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
     constraints: typing.List[Constraint]
     match_type: SegmentMatchType = pydantic.Field(alias="matchType")
```

### Comparing `flipt-0.2.6/src/flipt/resources/segments/types/segment_create_request.py` & `flipt-0.2.7/src/flipt/resources/segments/types/segment_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/segments/types/segment_list.py` & `flipt-0.2.7/src/flipt/resources/segments/types/segment_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/segments/types/segment_match_type.py` & `flipt-0.2.7/src/flipt/resources/segments/types/segment_match_type.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/segments/types/segment_update_request.py` & `flipt-0.2.7/src/flipt/resources/segments/types/segment_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/variants/client.py` & `flipt-0.2.7/src/flipt/resources/variants/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/variants/types/variant.py` & `flipt-0.2.7/src/flipt/resources/rollouts/types/rollout_segment.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,17 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class Variant(pydantic.BaseModel):
-    id: str
-    flag_key: str = pydantic.Field(alias="flagKey")
-    key: str
-    name: str
-    description: str
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    attachment: str
+class RolloutSegment(pydantic.BaseModel):
+    segment_key: str = pydantic.Field(alias="segmentKey")
+    value: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.6/src/flipt/resources/variants/types/variant_create_request.py` & `flipt-0.2.7/src/flipt/resources/variants/types/variant_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.6/src/flipt/resources/variants/types/variant_update_request.py` & `flipt-0.2.7/src/flipt/resources/rules/types/rule.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...distributions.types.distribution import Distribution
 
 
-class VariantUpdateRequest(pydantic.BaseModel):
-    key: str
-    name: typing.Optional[str]
-    description: typing.Optional[str]
-    attachment: typing.Optional[str]
+class Rule(pydantic.BaseModel):
+    id: str
+    namespace_key: str = pydantic.Field(alias="namespaceKey")
+    flag_key: str = pydantic.Field(alias="flagKey")
+    segment_key: str = pydantic.Field(alias="segmentKey")
+    distributions: typing.List[Distribution]
+    rank: int
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `flipt-0.2.6/PKG-INFO` & `flipt-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipt
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


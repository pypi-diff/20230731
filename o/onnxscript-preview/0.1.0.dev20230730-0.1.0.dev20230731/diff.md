# Comparing `tmp/onnxscript-preview-0.1.0.dev20230730.tar.gz` & `tmp/onnxscript-preview-0.1.0.dev20230731.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-preview-0.1.0.dev20230730.tar", last modified: Sun Jul 30 00:17:07 2023, max compression
+gzip compressed data, was "onnxscript-preview-0.1.0.dev20230731.tar", last modified: Mon Jul 31 00:16:14 2023, max compression
```

## Comparing `onnxscript-preview-0.1.0.dev20230730.tar` & `onnxscript-preview-0.1.0.dev20230731.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.830186 onnxscript-preview-0.1.0.dev20230730/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-30 00:17:07.830186 onnxscript-preview-0.1.0.dev20230730/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.798184 onnxscript-preview-0.1.0.dev20230730/onnxscript/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.802185 onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/param_manipulation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/analysis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.802185 onnxscript-preview-0.1.0.dev20230730/onnxscript/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/backend/onnx_backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/backend/onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/backend/onnx_export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    60982 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/converter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.794184 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.802185 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.810185 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/evaluator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.794184 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.794184 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.810185 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.814185 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28455 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/graph_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/graph_building_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.814185 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   230758 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)    75582 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/tensor_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/irbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.814185 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.818186 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)   152497 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 runner    (1001) docker     (123)    53435 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 runner    (1001) docker     (123)   156522 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 runner    (1001) docker     (123)    42746 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 runner    (1001) docker     (123)   139640 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 runner    (1001) docker     (123)    69354 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 runner    (1001) docker     (123)    74270 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 runner    (1001) docker     (123)    33248 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 runner    (1001) docker     (123)    49053 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 runner    (1001) docker     (123)    58408 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/sourceinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tensor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.822186 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.822186 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/common/onnx_script_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/eager_mode_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/eager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/external_tensor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.794184 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/function_libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.822186 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/function_libs/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/function_libs/torch_lib/ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    75865 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.822186 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/attr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/gemmgelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/gemmgelu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/if_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/onnxfns1A_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/onnxfns2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/onnxfns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/ort_custom_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/if_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/loop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.826186 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/attrref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/cast_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/different_opset.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/eager_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/eg1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/graph_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/if_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/loops_break.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/loops_while.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/m1.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/onnxfns1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/onnxfns1A.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/onnxfns2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/opt_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/opt_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/renaming.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/signal_dft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/subfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/type_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/onnx_types_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/operator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/type_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/type_annotation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24387 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript/values_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:17:07.826186 onnxscript-preview-0.1.0.dev20230730/onnxscript_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-30 00:17:07.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-07-30 00:17:07.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 00:17:07.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-30 00:17:07.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 00:17:07.000000 onnxscript-preview-0.1.0.dev20230730/onnxscript_preview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-30 00:16:59.000000 onnxscript-preview-0.1.0.dev20230730/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 00:17:07.830186 onnxscript-preview-0.1.0.dev20230730/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-30 00:16:54.000000 onnxscript-preview-0.1.0.dev20230730/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.663480 onnxscript-preview-0.1.0.dev20230731/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-31 00:16:14.663480 onnxscript-preview-0.1.0.dev20230731/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.639480 onnxscript-preview-0.1.0.dev20230731/onnxscript/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.639480 onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/param_manipulation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/analysis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.639480 onnxscript-preview-0.1.0.dev20230731/onnxscript/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/backend/onnx_backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/backend/onnx_export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60982 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/converter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.631480 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.639480 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.647480 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/evaluator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.631480 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.631480 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.647480 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.647480 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28455 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/graph_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/graph_building_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.651480 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   230758 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75582 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/tensor_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/irbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.651480 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.655480 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)   152497 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53435 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156522 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42746 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139640 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69354 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74270 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33248 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49053 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58408 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/sourceinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tensor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.655480 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.655480 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/common/onnx_script_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/eager_mode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/eager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/external_tensor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.631480 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/function_libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.659480 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/function_libs/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/function_libs/torch_lib/ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75865 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.659480 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/attr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/gemmgelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/gemmgelu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/if_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/onnxfns1A_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/onnxfns2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/onnxfns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/ort_custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/if_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/loop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.663480 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/attrref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/cast_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/different_opset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/eager_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/eg1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/graph_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/if_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/loops_break.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/loops_while.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/m1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/onnxfns1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/onnxfns1A.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/onnxfns2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/opt_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/opt_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/renaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/signal_dft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/subfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/type_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/onnx_types_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/operator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/type_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/type_annotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24387 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript/values_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:16:14.663480 onnxscript-preview-0.1.0.dev20230731/onnxscript_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-31 00:16:14.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-07-31 00:16:14.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:16:14.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 00:16:14.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 00:16:14.000000 onnxscript-preview-0.1.0.dev20230731/onnxscript_preview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-31 00:16:07.000000 onnxscript-preview-0.1.0.dev20230731/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:16:14.663480 onnxscript-preview-0.1.0.dev20230731/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-31 00:16:04.000000 onnxscript-preview-0.1.0.dev20230731/setup.py
```

### Comparing `onnxscript-preview-0.1.0.dev20230730/LICENSE` & `onnxscript-preview-0.1.0.dev20230731/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/PKG-INFO` & `onnxscript-preview-0.1.0.dev20230731/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript-preview
-Version: 0.1.0.dev20230730
+Version: 0.1.0.dev20230731
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-preview-0.1.0.dev20230730/README.md` & `onnxscript-preview-0.1.0.dev20230731/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/__init__.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/ast_utils.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/autocast.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/param_manipulation.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/param_manipulation_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/param_manipulation_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/runtime_typing.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/_internal/version_utils.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/analysis.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/analysis_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/analysis_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/backend/onnx_backend.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/backend/onnx_backend_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/backend/onnx_backend_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/backend/onnx_export.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/backend/onnx_export_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/backend/onnx_export_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/converter.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/converter_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/converter_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/context.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/diagnostics/infra/utils.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/evaluator.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/evaluator_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/evaluator_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/graph_building_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/graph_building_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/irbuilder.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/main.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/__init__.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/onnx_types.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/sourceinfo.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tensor.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tensor_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tensor_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/testing.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/testing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/common/onnx_script_test_case.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/common/onnx_script_test_case.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/eager_mode_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/eager_mode_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/eager_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/eager_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/external_tensor_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/external_tensor_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/function_libs/torch_lib/ops_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/function_libs/torch_lib/ops_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/function_libs/torch_lib/ops_test_common.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/function_libs/torch_lib/ops_test_common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/function_libs/torch_lib/ops_test_data.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/function_libs/torch_lib/ops_test_data.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/attr_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/attr_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/gemmgelu.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/gemmgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/gemmgelu_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/gemmgelu_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/if_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/if_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/onnxfns1A_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/onnxfns1A_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/onnxfns2_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/onnxfns2_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/onnxfns_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/onnxfns_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/functions/ort_custom_ops.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/functions/ort_custom_ops.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/if_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/if_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/loop_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/loop_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/attrref.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/attrref.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/cast_like.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/cast_like.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/different_opset.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/different_opset.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/dropout.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/dropout.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/eager_op.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/eager_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/eg1.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/eg1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/getitem.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/getitem.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/graph_attr.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/graph_attr.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/identity.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/identity.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/if_statement.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/if_statement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/loops_break.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/loops_break.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/loops_while.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/loops_while.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/onnxfns1.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/onnxfns1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/onnxfns1A.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/onnxfns1A.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/onnxfns2.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/onnxfns2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/opt_input.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/opt_input.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/opt_output.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/opt_output.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/renaming.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/renaming.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/sequences.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/sequences.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/signal_dft.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/signal_dft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/subfunction.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/subfunction.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/models/type_double.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/models/type_double.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/onnx_types_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/onnx_types_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/tests/operator_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/tests/operator_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/type_annotation.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/type_annotation_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/type_annotation_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/utils.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/values.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript/values_test.py` & `onnxscript-preview-0.1.0.dev20230731/onnxscript/values_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript_preview.egg-info/PKG-INFO` & `onnxscript-preview-0.1.0.dev20230731/onnxscript_preview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript-preview
-Version: 0.1.0.dev20230730
+Version: 0.1.0.dev20230731
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-preview-0.1.0.dev20230730/onnxscript_preview.egg-info/SOURCES.txt` & `onnxscript-preview-0.1.0.dev20230731/onnxscript_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/pyproject.toml` & `onnxscript-preview-0.1.0.dev20230731/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230730/setup.py` & `onnxscript-preview-0.1.0.dev20230731/setup.py`

 * *Files identical despite different names*


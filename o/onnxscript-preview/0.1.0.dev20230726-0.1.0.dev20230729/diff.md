# Comparing `tmp/onnxscript-preview-0.1.0.dev20230726.tar.gz` & `tmp/onnxscript-preview-0.1.0.dev20230729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-preview-0.1.0.dev20230726.tar", last modified: Wed Jul 26 00:09:23 2023, max compression
+gzip compressed data, was "onnxscript-preview-0.1.0.dev20230729.tar", last modified: Sat Jul 29 00:15:13 2023, max compression
```

## Comparing `onnxscript-preview-0.1.0.dev20230726.tar` & `onnxscript-preview-0.1.0.dev20230729.tar`

### file list

```diff
@@ -1,216 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.186549 onnxscript-preview-0.1.0.dev20230726/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-26 00:09:23.186549 onnxscript-preview-0.1.0.dev20230726/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.166549 onnxscript-preview-0.1.0.dev20230726/onnxscript/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.166549 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/feature_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/param_manipulation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/analysis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/autocast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.166549 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    59491 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/converter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.158549 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.166549 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.174548 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/evaluator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.158549 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.158549 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.174548 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.174548 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/graph_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/graph_building_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.174548 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   226462 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)    75574 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/tensor_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/irbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.174548 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.178549 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)   152497 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 runner    (1001) docker     (123)    53435 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 runner    (1001) docker     (123)   156522 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 runner    (1001) docker     (123)    42746 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 runner    (1001) docker     (123)   139640 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 runner    (1001) docker     (123)    69354 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 runner    (1001) docker     (123)    74270 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 runner    (1001) docker     (123)    33248 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 runner    (1001) docker     (123)    49053 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 runner    (1001) docker     (123)    58408 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/sourceinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tensor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.178549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.178549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/common/onnx_script_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/eager_mode_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/eager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/external_tensor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.162549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.182549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    72345 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.182549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/attr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/gemmgelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/gemmgelu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/if_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns1A_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/ort_custom_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/if_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/loop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.186549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/attrref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/cast_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/different_opset.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/eager_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/eg1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/graph_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/if_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/loops_break.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/loops_while.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/m1.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns1A.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/opt_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/opt_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/renaming.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/signal_dft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/subfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/type_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/onnx_types_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/operator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/type_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/type_annotation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24387 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/values_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.186549 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-26 00:09:23.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-26 00:09:23.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:09:23.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 00:09:23.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 00:09:23.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-26 00:09:16.000000 onnxscript-preview-0.1.0.dev20230726/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 00:09:23.186549 onnxscript-preview-0.1.0.dev20230726/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.891994 onnxscript-preview-0.1.0.dev20230729/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-29 00:15:13.891994 onnxscript-preview-0.1.0.dev20230729/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.867994 onnxscript-preview-0.1.0.dev20230729/onnxscript/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.867994 onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/param_manipulation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/analysis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.867994 onnxscript-preview-0.1.0.dev20230729/onnxscript/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/backend/onnx_backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/backend/onnx_export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60982 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/converter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.859994 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.867994 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.875994 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/evaluator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.859994 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.859994 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.875994 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.879994 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28455 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/graph_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/graph_building_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.879994 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   230758 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75582 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/tensor_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/irbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.879994 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.883994 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)   152497 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53435 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156522 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42746 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139640 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69354 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74270 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33248 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49053 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58408 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/sourceinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tensor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.887994 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.887994 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/common/onnx_script_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/eager_mode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/eager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/external_tensor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.859994 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/function_libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.887994 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/function_libs/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/function_libs/torch_lib/ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75865 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.887994 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/attr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/gemmgelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/gemmgelu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/if_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/onnxfns1A_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/onnxfns2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/onnxfns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/ort_custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/if_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/loop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.891994 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/attrref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/cast_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/different_opset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/eager_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/eg1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/graph_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/if_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/loops_break.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/loops_while.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/m1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/onnxfns1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/onnxfns1A.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/onnxfns2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/opt_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/opt_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/renaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/signal_dft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/subfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/type_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/onnx_types_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/operator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/type_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/type_annotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24387 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript/values_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:15:13.891994 onnxscript-preview-0.1.0.dev20230729/onnxscript_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-29 00:15:13.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-07-29 00:15:13.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:15:13.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 00:15:13.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 00:15:13.000000 onnxscript-preview-0.1.0.dev20230729/onnxscript_preview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-29 00:15:06.000000 onnxscript-preview-0.1.0.dev20230729/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:15:13.891994 onnxscript-preview-0.1.0.dev20230729/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-29 00:15:02.000000 onnxscript-preview-0.1.0.dev20230729/setup.py
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/LICENSE` & `onnxscript-preview-0.1.0.dev20230729/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/PKG-INFO` & `onnxscript-preview-0.1.0.dev20230729/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: onnxscript-preview
-Version: 0.1.0.dev20230726
-Summary: Authoring ONNX functions in Python
+Version: 0.1.0.dev20230729
+Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,26 +21,26 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Repository, https://github.com/onnx/onnxscript
+Project-URL: Repository, https://github.com/microsoft/onnxscript
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ----
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/README.md` & `onnxscript-preview-0.1.0.dev20230729/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/__init__.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/ast_utils.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/param_manipulation.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/param_manipulation_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/param_manipulation_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/runtime_typing.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/version_utils.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/analysis.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,49 +33,53 @@
     else:
         children = ast.iter_child_nodes(expr)  # type: ignore[assignment]
     for c in children:
         result = result | used_vars(c)
     return result
 
 
-def local_defs(lhs: ast.expr) -> Set[str]:
-    """Utility function to return set of assigned/defined
-    variables in the lhs of an assignment statement.
-    """
+def lhs_vars(lhs: ast.expr) -> Set[str]:
+    """Return set of assigned variables in the lhs of an assignment statement."""
 
     def get_id(e):
         assert isinstance(e, ast.Name), "Only simple assignments supported."
         return e.id
 
     if isinstance(lhs, ast.Tuple):
         return {get_id(x) for x in lhs.elts}
     return {get_id(lhs)}
 
 
-def defs(stmt: ast.stmt) -> Set[str]:
-    """Return the set of all variables that may be defined (assigned to) in an
-    execution of input stmt.
+def assigned_vars(
+    stmt: ast.stmt | list[ast.stmt], formatter: sourceinfo.Formatter
+) -> Set[str]:
+    """Return the set of all variables that may be assigned to in an execution of input stmt
+    or sequence of statements.
     """
 
-    def block_defs(block: Sequence[ast.stmt]) -> Set[str]:
+    def assigned_in_block(block: Sequence[ast.stmt]) -> Set[str]:
         result: set[Any] = set()
         for s in block:
-            result = result | defs(s)
+            result = result | assigned_vars(s, formatter)
         return result
 
     if isinstance(stmt, ast.Assign):
-        return local_defs(stmt.targets[0])
+        return lhs_vars(stmt.targets[0])
     if isinstance(stmt, ast.AnnAssign):
-        return local_defs(stmt.target)
+        return lhs_vars(stmt.target)
     if isinstance(stmt, ast.Return):
         return set()
     if isinstance(stmt, ast.If):
-        return block_defs(stmt.body) | block_defs(stmt.orelse)
+        return assigned_in_block(stmt.body) | assigned_in_block(stmt.orelse)
+    if isinstance(stmt, ast.For):
+        return assigned_in_block(stmt.body) | {get_loop_var(stmt, formatter)}
+    if isinstance(stmt, ast.While):
+        return assigned_in_block(stmt.body)
     if isinstance(stmt, list):
-        return block_defs(stmt)
+        return assigned_in_block(stmt)
     if isinstance(stmt, ast.Break):
         return set()
     if ast_utils.is_print_call(stmt):
         return set()
     raise ValueError(f"Unsupported statement type {type(stmt)!r}.")
 
 
@@ -94,17 +98,17 @@
     def do_visit(stmt: ast.stmt, live_out: Set[str]) -> Set[str]:
         def visitBlock(block: Sequence[ast.stmt], live_out: Set[str]) -> Set[str]:
             for s in reversed(block):
                 live_out = visit(s, live_out)
             return live_out
 
         if isinstance(stmt, ast.Assign):
-            return live_out.difference(local_defs(stmt.targets[0])) | used_vars(stmt.value)
+            return live_out.difference(lhs_vars(stmt.targets[0])) | used_vars(stmt.value)
         if isinstance(stmt, ast.AnnAssign):
-            return live_out.difference(local_defs(stmt.target)) | used_vars(stmt.value)
+            return live_out.difference(lhs_vars(stmt.target)) | used_vars(stmt.value)
         if isinstance(stmt, ast.Return):
             return used_vars(stmt.value)
         if isinstance(stmt, ast.If):
             live1 = visitBlock(stmt.body, live_out)
             live2 = visitBlock(stmt.orelse, live_out)
             return live1 | live2 | used_vars(stmt.test)
         if isinstance(stmt, ast.For):
@@ -166,17 +170,17 @@
     def visitBlock(block: Sequence[ast.stmt], live_out: Set[str]) -> Set[str]:
         for stmt in reversed(block):
             live_out = visit(stmt, live_out)
         return live_out
 
     def visit(stmt: ast.stmt, live_out: Set[str]) -> Set[str]:
         if isinstance(stmt, ast.Assign):
-            return live_out.difference(local_defs(stmt.targets[0])) | used_vars(stmt.value)
+            return live_out.difference(lhs_vars(stmt.targets[0])) | used_vars(stmt.value)
         if isinstance(stmt, ast.AnnAssign):
-            return live_out.difference(local_defs(stmt.target)) | used_vars(stmt.value)
+            return live_out.difference(lhs_vars(stmt.target)) | used_vars(stmt.value)
         if isinstance(stmt, ast.Return):
             return used_vars(stmt.value)
         if isinstance(stmt, ast.If):
             live1 = visitBlock(stmt.body, live_out)
             live2 = visitBlock(stmt.orelse, live_out)
             return (live1 | live2) | used_vars(stmt.test)
         if ast_utils.is_print_call(stmt):
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/analysis_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/analysis_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -159,9 +159,61 @@
                 return y
 
             return op.Dummy(x)
 
         self.assertUses(f, {"x"})
 
 
+class TestAssignedVarAnalysis(unittest.TestCase):
+    def assert_assigned_vars(self, f, expected: set[str]):
+        source, parse_tree = ast_utils.get_src_and_ast(f)
+        result = analysis.assigned_vars(parse_tree.body, formatter(source))
+        self.assertEqual(result, expected)
+
+    def test_basic_defs(self):
+        def f(x):
+            x = x + 1
+            y = x + 2
+            return y
+
+        self.assert_assigned_vars(f, {"x", "y"})
+
+    def test_if_defs(self):
+        def f(x):
+            if x > 1:
+                y = x + 1
+                z = 2 * y
+            else:
+                t = x + 2
+                z = 3 * t
+            return z
+
+        self.assert_assigned_vars(f, {"z", "y", "t"})
+
+    def test_loop_defs(self):
+        def f(x):
+            sum = 0
+            while x > 0:
+                x = x - 1
+                square = x * x
+                sum = sum + square
+            return sum
+
+        self.assert_assigned_vars(f, {"sum", "x", "square"})
+
+    def test_if_loop_defs(self):
+        def f(x):
+            if x > 0:
+                sum = 0
+                while x > 0:
+                    x = x - 1
+                    square = x * x
+                    sum = sum + square
+            else:
+                sum = 0
+            return sum
+
+        self.assert_assigned_vars(f, {"sum", "x", "square"})
+
+
 if __name__ == "__main__":
     unittest.main(verbosity=2)
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/autocast.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/_internal/autocast.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,14 +60,58 @@
         return helper.make_tensor(tensor_name, onnx_type, [], [int(pyvalue)])
     if onnx_type is onnx.TensorProto.STRING:
         return helper.make_tensor(tensor_name, onnx_type, [], vals=[pyvalue.encode("utf-8")])
 
     return helper.make_tensor(tensor_name, onnx_type, [], [pyvalue])
 
 
+_REPEATED_ATTRIBUTE_TYPES = frozenset(
+    {
+        onnx.AttributeProto.FLOATS,
+        onnx.AttributeProto.INTS,
+        onnx.AttributeProto.STRINGS,
+        onnx.AttributeProto.TENSORS,
+        onnx.AttributeProto.GRAPHS,
+        onnx.AttributeProto.SPARSE_TENSORS,
+        onnx.AttributeProto.TYPE_PROTOS,
+    }
+)
+
+
+def pyvalue_to_onnx_attribute(
+    key: str,
+    value: Any,
+    name_generator: Callable[[], str],
+    attr_type: Optional[onnx.AttributeProto.AttributeType] = None,
+) -> onnx.AttributeProto:
+    """Helper function to create an ONNX AttributeProto.
+
+    This is a refinement of onnx.helper.make_attribute that works with ONNX Script
+    conventions for allowed types for attribute-values. In particular, it allows
+    * Empty lists as attribute values, provided the attribute type is specified
+    and is a list type.
+    * Scalar-values like 1.0 as well as lists like [1, -1] to be specified
+    when the attribute type is TensorProto by automatically converting the value
+    into a 0-D or 1-D tensor respectively.
+    """
+    if isinstance(value, list) and not value:
+        # Empty list value:
+        if attr_type is None:
+            raise ValueError("Attribute type must be specified for empty list value.")
+        if attr_type not in _REPEATED_ATTRIBUTE_TYPES:
+            raise ValueError("Empty list value is only allowed for repeated attribute types.")
+        return onnx.AttributeProto(name=key, type=attr_type)
+    elif attr_type == onnx.AttributeProto.TENSOR and not isinstance(value, onnx.TensorProto):
+        return onnx.AttributeProto(
+            name=key, type=attr_type, t=pyvalue_to_onnx_tensor(name_generator(), value)
+        )
+    else:
+        return onnx.helper.make_attribute(key, value)
+
+
 # Utilities to convert python values into onnxscript tensors.
 
 
 def _promotable(x) -> bool:
     """Checks if a runtime parameter value needs to be promoted into an onnxscript value.
     This is the runtime-equivalent of the promotion of literal constants into ONNX values
     in the static converter.
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_backend.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_backend_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/backend/onnx_backend_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_export.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_export_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/backend/onnx_export_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/converter.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     Tuple,
     Union,
 )
 
 import onnx
 
 import onnxscript
-from onnxscript import analysis, autocast, irbuilder, onnx_types, sourceinfo
+from onnxscript import analysis, irbuilder, onnx_types, sourceinfo
 from onnxscript import type_annotation as ta
 from onnxscript import values
-from onnxscript._internal import ast_utils, param_manipulation
+from onnxscript._internal import ast_utils, autocast, param_manipulation
 
 PY_VERSION_GE_39 = ast_utils.PY_VERSION_GE_39
 
 
 logger = logging.getLogger("onnxscript")
 
 
@@ -299,14 +299,26 @@
         r = candidate
         while r in self._used_vars:
             r = f"{candidate}_{self._nextvar}"
             self._nextvar = self._nextvar + 1
         self._used_vars.add(r)
         return r
 
+    def make_onnx_attr(
+        self, attrname: str, attrval: Any, attrtype: Optional[int] = None
+    ) -> irbuilder.IRAttributeValue:
+        def tensor_name_generator() -> str:
+            """Return name to be used for tensor, if we need to create one."""
+            return self.generate_unique_name(f"attr_{attrname}")
+
+        proto = autocast.pyvalue_to_onnx_attribute(
+            attrname, attrval, tensor_name_generator, attrtype
+        )
+        return self.ir_builder.make_attr(proto)
+
     def to_onnx_attr_ref(
         self, val: values.AttrRef, info: Optional[sourceinfo.SourceInfo]
     ) -> irbuilder.IRAttributeValue:
         pytype = val.typeinfo
         attrtype = ta.pytype_to_attrtype(pytype)
         attrname = None
         if attrtype is onnx.AttributeProto.FLOAT:
@@ -334,15 +346,15 @@
             attr = self.to_onnx_attr_ref(val, info)
             self.emit([result], values.Op(self.default_opset, "Constant"), [], [attr])
             if ta.base_type_is_bool(val.typeinfo):
                 # ONNX attributes use an int-encoding for bools, but ONNX tensor types
                 # distinguish between int and bool. So we cast the int tensor to a bool tensor,
                 # to promote a (python) bool attribute to a ONNX bool tensor.
                 result_as_bool = self.generate_unique_name(result + "_as_bool")
-                cast_attr = self.ir_builder.make_attr("to", onnx_types.BOOL.dtype)
+                cast_attr = self.make_onnx_attr("to", onnx_types.BOOL.dtype)
                 self.emit(
                     [result_as_bool],
                     values.Op(self.default_opset, "Cast"),
                     [result],
                     [cast_attr],
                 )
                 return Variable(result_as_bool, True)
@@ -405,15 +417,15 @@
             else:
                 suggested_name = "const"
         ovar = self.generate_unique_name(suggested_name)
         try:
             tensor = autocast.pyvalue_to_onnx_tensor(ovar, pyvalue)
         except ValueError as e:
             fail(info.msg(str(e)))
-        attr = self.ir_builder.make_attr("value", tensor)
+        attr = self.make_onnx_attr("value", tensor)
         self.emit([ovar], values.Op(self.default_opset, "Constant"), [], [attr])
         return Variable(ovar, True)
 
     def emit_copy(self, original_var: str, suggested_name: str) -> str:
         """Emits a copy statement, using the ONNX Identity operator."""
         new_var = self.generate_unique_name(suggested_name)
         self.emit([new_var], "Identity", [original_var])
@@ -467,53 +479,72 @@
                     expr,
                     f"Missing names, globals contains {list(self.globals)!r}, "
                     f"locals {list(locals)!r}.",
                 )
             ) from e
 
     def translate_attr(
-        self, attr_name: str, expr: ast.AST
+        self,
+        attr_name: str,
+        expr: ast.AST,
+        attr_meta: Optional[onnx.defs.OpSchema.Attribute] = None,
     ) -> Optional[irbuilder.IRAttributeValue]:
         """Translate an attribute-value specification of the form `attr_name=<expr>`
         in a call to an op. expr is an AST. The following cases are supported:
         * Expr evaluates to a script-time constant (a python-value) that can be mapped
         into an ONNX attribute value, or
         * Expr evaluates to None, in which case None is returned, or
         * Expr must be an attribute-reference, that is a name representing an
         attribute-parameter of a containing function.
         """
+
         if isinstance(expr, ast.Name):
             val = self.lookup(expr.id, self.source_of(expr))
             if isinstance(val, values.AttrRef):
-                return self.ir_builder.make_attr_ref(attr_name, val.value, val.typeinfo)
+                attr_ref = self.ir_builder.make_attr_ref(attr_name, val.value, val.typeinfo)
+                if attr_meta is not None and (attr_ref.type != attr_meta.type):
+                    self.fail(
+                        expr,
+                        f"Attribute type '{attr_ref.type}' does not match expected type '{attr_meta.type}'",
+                    )
+                return attr_ref
             if isinstance(val, irbuilder.IRFunction):
                 # Check that outer-scope variables referenced by function have same value
                 # at function-definition site and use-as-attribute site, to avoid errors.
                 for pyvar, previous in val.outer_scope_variables:
                     current = self.lookup(pyvar, self.source_of(expr))
                     if current.value != previous.value:
                         self.fail(
                             expr,
-                            f"Outer scope variable {pyvar} referenced by function "
-                            f"{expr.id!r} modified.",
+                            f"Outer scope variable '{pyvar}' referenced by function "
+                            f"'{expr.id!r}' modified.",
                         )
 
                 # Create GraphProto attribute
                 val = val.to_graph_proto()
         else:
             val = self.eval_constant_expr(expr)
 
         # In ONNX, there is no way to explicitly specify a None value for an attribute.
         # Instead, the attribute must be omitted from the attribute list.
         # Hence, we do not create an attribute-proto if the value is None.
         # The caller is responsible for omitting such attribute-values from the list of attributes
         # in a NodeProto.
         if val is None:
+            if attr_meta and attr_meta.required:
+                self.fail(expr, "Attribute '{attr_name}' is required.")
             return None
-        return self.ir_builder.make_attr(attr_name, val)
+        attr_type = attr_meta.type if attr_meta else None
+        attr = self.make_onnx_attr(attr_name, val, attr_type)
+        if attr_meta and (attr.type != attr_meta.type):
+            self.fail(
+                expr,
+                f"Attribute type '{attr.type}' does not match expected type '{attr_meta.type}'",
+            )
+        return attr
 
     def translate_docstring(self, node: ast.Expr) -> None:
         if hasattr(node.value, "value"):
             # python 3.8+
             return self.emit_docstring(node.value.value)
         raise TypeError(
             f"Unexpected type {type(node)!r} for node. Unsupoorted version of python."
@@ -726,15 +757,15 @@
                 inputs = translate_slice(element)
                 starts.append(inputs[0])
                 ends.append(inputs[1])
                 axes.append(axis_var.name)
                 steps.append(inputs[2])
 
             if len(starts) > 1:
-                axis_0_attr = self.ir_builder.make_attr("axis", 0)
+                axis_0_attr = self.make_onnx_attr("axis", 0)
                 start_name = self.generate_unique_name(f"{var_name}_start")
                 self.emit([start_name], "Concat", starts, [axis_0_attr])
 
                 end_name = self.generate_unique_name(f"{var_name}_end")
                 self.emit([end_name], "Concat", ends, [axis_0_attr])
 
                 axes_name = self.generate_unique_name(f"{var_name}_axis")
@@ -773,15 +804,15 @@
         else:
             result = var_name
         non_scalar_indices.extend(scalar_indices)
         if non_scalar_indices:
             last_axis, _ = non_scalar_indices[-1]
         for axis, index_expr in non_scalar_indices:
             index_value = self.translate_expr(index_expr)
-            axis_attr = self.ir_builder.make_attr("axis", axis)
+            axis_attr = self.make_onnx_attr("axis", axis)
             # use Gather to perform indexing
             # Assign gathered value to either temporary or final target
             if axis != last_axis:  # use temporary to store result of Gather
                 gathered = self.generate_unique_name(f"{var_name}_axis_{axis}")
             else:  # store result of Gather in final target
                 gathered = target
             self.emit([gathered], "Gather", [str(result), index_value], [axis_attr])
@@ -797,15 +828,18 @@
         # Otherwise, we map named arguments to attributes and positional arguments to inputs.
         if param_schemas:
             kwargs = {x.arg: x.value for x in node.keywords}
             args, attrs = param_manipulation.separate_input_attributes_from_arguments(
                 param_schemas, node.args, kwargs, fill_defaults=False
             )
             args = [self.translate_opt_expr(x) for x in args]
-            attrs = [self.translate_attr(x, y) for x, y in attrs.items()]
+            attrs = [
+                self.translate_attr(x, y, callee.op_schema.attributes[x])
+                for x, y in attrs.items()
+            ]
         else:
             args = [self.translate_opt_expr(x) for x in node.args]
             attrs = [self.translate_attr(x.arg, x.value) for x in node.keywords]
         args = autocast.static_cast_inputs(self, callee.op_schema, args)
 
         # In ONNX, there is no way to explicitly specify a None value for an attribute.
         # Instead, the attribute must be omitted from the attribute list.
@@ -824,15 +858,15 @@
 
         attr = []
         if isinstance(node.op, ast.Mod) and self.is_constant_expr(node.right):
             # specific case X % f where f is a float.
             # attribute fmod=1 is added in that case.
             cst = self.eval_constant_expr(node.right)
             if isinstance(cst, float):
-                attr = [self.ir_builder.make_attr("fmod", 1)]
+                attr = [self.make_onnx_attr("fmod", 1)]
 
         op = values.Op(self.default_opset, primop_map[op])
         left, right = self._cast_like_binary_expression(
             op, self.translate_expr(node.left), self.translate_expr(node.right)
         )
         return op, [left, right], attr
 
@@ -898,14 +932,15 @@
                 return val
             self.fail(node, f"'{node.id}' is not an instance of type Opset but {type(val)}.")
         elif isinstance(node, ast.Attribute):
             self.fail(node, "Nested module unimplemented.")  # TODO
         else:
             self.fail(node, "Invalid opset expression.")
 
+    # pylint: enable=inconsistent-return-statements
     def translate_callee_expr(self, node: ast.AST) -> values.Op:  # pylint: disable=R1710
         """Return an Op"""
         if isinstance(node, ast.Attribute):
             module = self.translate_opset_expr(node.value)
             self.set_default_opset(module, node)
             opname = node.attr
             if opname in module:
@@ -1063,27 +1098,29 @@
             check_num_outputs(len(val.elts))
             return [ret(exp, i, str(i)) for i, exp in enumerate(val.elts)]
         check_num_outputs(1)
         return ret(val, 0, "")
 
     def translate_if_stmt(self, stmt: ast.If) -> None:
         if hasattr(stmt, "live_out"):
-            live_defs = list(stmt.live_out.intersection(analysis.defs(stmt)))
+            live_defs = list(
+                stmt.live_out.intersection(analysis.assigned_vars(stmt, self.message))
+            )
         else:
-            live_defs = list(analysis.defs(stmt))
+            live_defs = list(analysis.assigned_vars(stmt, self.message))
         test = self.translate_expr(stmt.test, "cond").name
         lineno = self.source_of(stmt).lineno
         thenGraph, sub_fct_then = self.translate_block(
             stmt.body, f"thenGraph_{lineno}", live_defs, parent_stmt=stmt
         )
-        thenAttr = self.ir_builder.make_attr("then_branch", thenGraph)
+        thenAttr = self.make_onnx_attr("then_branch", thenGraph)
         elseGraph, sub_fct_else = self.translate_block(
             stmt.orelse, f"elseGraph_{lineno}", live_defs, parent_stmt=stmt
         )
-        elseAttr = self.ir_builder.make_attr("else_branch", elseGraph)
+        elseAttr = self.make_onnx_attr("else_branch", elseGraph)
 
         def rename(x):
             r = self.generate_unique_name(x)
             self.bind(
                 x,
                 values.Dynamic(r, values.DynamicKind.Intermediate, self.source_of(stmt)),
             )
@@ -1144,15 +1181,15 @@
             o_cond_var = None
             # we need to go through all the instructions to see
             # which instruction defines the condition test.id
         else:
             self.fail(loop_stmt, f"Unexpected loop type {type(loop_stmt)!r}.")
         # analyze loop body
         exposed_uses = analysis.exposed_uses(loop_stmt.body, self.message)
-        vars_def_in_loop = analysis.defs(loop_stmt.body)
+        vars_def_in_loop = analysis.assigned_vars(loop_stmt.body, self.message)
         loop_state_vars = vars_def_in_loop.intersection(exposed_uses | loop_stmt.live_out)
         scan_outputs = set()  # TODO
         outputs = list(loop_state_vars | scan_outputs)
 
         # loop-condition:
         o_true = self.emit_const(True, "true", self.source_of(loop_stmt))
         # o_loop_bound = self.emit_const(3, "loop_bound")
@@ -1262,15 +1299,15 @@
             )
         body = self.exit_scope()
         inputs = [o_loop_bound, o_true] + [
             self.py_var_to_onnx_var(pv, self.source_of(loop_stmt)).name
             for pv in loop_state_vars
         ]
         graph, sub_functions = body.to_graph_and_functions()
-        attrs = [self.ir_builder.make_attr("body", graph)]
+        attrs = [self.make_onnx_attr("body", graph)]
         info = self.source_of(loop_stmt)
 
         def rename(x):
             r = self.generate_unique_name(x)
             self.bind(x, values.Dynamic(r, values.DynamicKind.Output, info))
             return r
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/converter_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/converter_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -603,10 +603,70 @@
         def if_then_else_expanded(flag: typing.List[bool], Y, Z):
             tmp1 = op.Constant(value_ints=flag)
             tmp2 = op.Cast(tmp1, to=9)
             return op.Where(tmp2, Y, Z)
 
         onnxscript.testing.assert_isomorphic(if_then_else, if_then_else_expanded)
 
+    def test_empty_ints_attribute(self):
+        @script()
+        def empty_ints():
+            return op.Constant(value_ints=[])
+
+        expected = np.array([], dtype=np.int64)
+        self.check_run(empty_ints, [], expected)
+
+    def test_empty_floats_attribute(self):
+        @script()
+        def empty_floats():
+            return op.Constant(value_floats=[])
+
+        expected = np.array([], dtype=np.float32)
+        self.check_run(empty_floats, [], expected)
+
+    def test_int_as_tensor_attribute(self):
+        @script()
+        def int_as_tensor():
+            return op.Constant(value=17)
+
+        expected = np.array(17, dtype=np.int64)
+        self.check_run(int_as_tensor, [], expected)
+
+    def test_int_list_as_tensor_attribute(self):
+        @script()
+        def int_list_as_tensor():
+            return op.Constant(value=[13, 17])
+
+        expected = np.array([13, 17], dtype=np.int64).reshape((2,))
+        self.check_run(int_list_as_tensor, [], expected)
+
+    def test_float_as_tensor_attribute(self):
+        @script()
+        def float_as_tensor():
+            return op.Constant(value=17.0)
+
+        expected = np.array([17], dtype=np.float32).reshape(())
+        self.check_run(float_as_tensor, [], expected)
+
+    def test_float_list_as_tensor_attribute(self):
+        @script()
+        def float_list_as_tensor():
+            return op.Constant(value=[13.0, 17.0])
+
+        expected = np.array([13, 17], dtype=np.float32).reshape((2,))
+        self.check_run(float_list_as_tensor, [], expected)
+
+    def test_loop_inside_if(self):
+        @script(default_opset=op)
+        def sum(n: INT64) -> INT64:
+            sum = op.Constant(value=0)
+            if n > 0:
+                for i in range(n):
+                    sum = sum + i
+            return sum
+
+        self.check_run(sum, [np.array(5, dtype=np.int64)], np.array(10, dtype=np.int64))
+        self.check_run(sum, [np.array(-5, dtype=np.int64)], np.array(0, dtype=np.int64))
+
 
 if __name__ == "__main__":
     unittest.main(verbosity=2)
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/context.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/utils.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/evaluator.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from __future__ import annotations
 
 import abc
 import contextlib
 import pprint
-import typing
 from typing import (
     Any,
     Callable,
     Mapping,
     Optional,
     Protocol,
     Sequence,
@@ -22,20 +21,16 @@
 
 import numpy as np
 import onnx
 import onnx.defs
 import onnx.helper
 from typing_extensions import TypeAlias
 
-from onnxscript import autocast, irbuilder, onnx_opset, tensor, utils, values
-from onnxscript._internal import feature_switch, param_manipulation
-
-if typing.TYPE_CHECKING:
-    import onnxruntime as ort
-
+from onnxscript import irbuilder, onnx_opset, tensor, utils, values
+from onnxscript._internal import autocast, param_manipulation
 
 UserModeValue: TypeAlias = Union[Optional[np.ndarray], Sequence["UserModeValue"]]
 
 EagerModeValue: TypeAlias = Union[Optional["tensor.Tensor"], Sequence["EagerModeValue"]]
 
 ExtendedModeValue: TypeAlias = Union[
     Optional["tensor.Tensor"],
@@ -362,35 +357,14 @@
             return len(scan_body.output)
         if schema.name == "Loop":
             loop_body = kwargs["body"]
             return len(loop_body.output) - 1
     return len(schema.outputs)
 
 
-_cache_models: dict[Any, ort.InferenceSession] = {}
-
-
-def _cache_(model, providers):
-    # Delay import onnxruntime so that onnxscript can be used without
-    # installing onnxruntime.
-    import onnxruntime as ort  # pylint: disable=import-outside-toplevel
-
-    serialized = model.SerializeToString()
-    if feature_switch.CACHE_ORT_SESSIONS:
-        key = serialized, tuple(providers)
-        if key in _cache_models:
-            return _cache_models[key]
-        session = ort.InferenceSession(serialized, providers=providers)
-        _cache_models[key] = session
-
-        return session
-
-    return ort.InferenceSession(serialized, providers=providers)
-
-
 def _os_to_ort_value(v):
     """Converts an onnxscript encoding of an ONNX value into the encoding used by ORT."""
     if isinstance(v, tensor.Tensor):
         return v.value
     if isinstance(v, list):
         return [_os_to_ort_value(x) for x in v]
     if v is None:
@@ -417,32 +391,45 @@
     schema: onnx.defs.OpSchema,
     args: Sequence[Any],
     kwargs: Mapping[str, Any],
     implicit_args=None,
 ):
     # Delay import onnxruntime so that onnxscript can be used without
     # installing onnxruntime.
+    import onnxruntime as ort  # pylint: disable=import-outside-toplevel
     from onnxruntime.capi.onnxruntime_pybind11_state import (  # pylint: disable=import-outside-toplevel
         Fail,
         InvalidArgument,
         InvalidGraph,
     )
 
     implicit_args = implicit_args or {}
     # Convert input values to ORT representation-type:
     args = [_os_to_ort_value(x) for x in args]
     implicit_args = {k: _os_to_ort_value(v) for k, v in implicit_args.items()}
 
+    # Utility to convert kwarg to ONNX AttributeProto:
+    def make_attr(key: str, value: Any) -> onnx.AttributeProto:
+        def make_tensor_name() -> str:
+            return f"attr_{key}"
+
+        return autocast.pyvalue_to_onnx_attribute(
+            key, value, make_tensor_name, schema.attributes[key].type
+        )
+
     # Construct ONNX model with a single op call:
     inputs = [_rename_io("input", i, arg) for i, arg in enumerate(args)]
 
     num_outputs = compute_num_outputs(schema, args, kwargs)
     outputs = [f"output{i}" for i in range(num_outputs)]
 
-    node = onnx.helper.make_node(schema.name, inputs, outputs, domain=schema.domain, **kwargs)
+    node = onnx.helper.make_node(schema.name, inputs, outputs, domain=schema.domain)
+    node.attribute.extend(
+        make_attr(key, value) for key, value in kwargs.items() if value is not None
+    )
     input_value_infos = utils.values_to_value_infos(zip(inputs, args))
     implicit_value_infos = utils.values_to_value_infos(implicit_args.items())
     output_value_infos = [
         onnx.helper.make_value_info(name, onnx.TypeProto()) for name in outputs
     ]
 
     graph = onnx.helper.make_graph(
@@ -451,17 +438,18 @@
     opset_id = onnx.helper.make_opsetid(schema.domain, schema.since_version)
     model = onnx.helper.make_model(
         graph,
         opset_imports=[opset_id],
         ir_version=irbuilder.select_ir_version(schema.since_version, domain=schema.domain),
     )
     model = onnx.shape_inference.infer_shapes(model)
-    # onnx.checker.check_model(model)
     try:
-        session = _cache_(model, ["CPUExecutionProvider"])
+        session = ort.InferenceSession(
+            model.SerializeToString(), providers=("CPUExecutionProvider",)
+        )
     except (Fail, InvalidGraph, InvalidArgument) as e:
         raise RuntimeError(
             f"Unable to create onnxruntime InferenceSession "
             f"for executing {schema.domain}.{schema.name} op "
             f"with onnx model\n{utils.proto2text(model)}"
         ) from e
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/evaluator_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/evaluator_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Graph building functions for torchscript graph backend."""
 from __future__ import annotations
 
 import logging
+import os
 import typing
 import warnings
 from typing import Any, Dict, Final, List, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import onnx
 import onnx.checker
@@ -85,14 +86,15 @@
     """A onnxscript tensor that wraps a torchscript Value."""
 
     def __init__(self, value: torch.Value):
         super().__init__(None)
         self._torch_value: torch.Value = value
         self._concrete_value: Optional[np.ndarray] = None
         self._shape: Optional[Tuple[int | None, ...]] = None
+        self._torch_dtype: Optional[torch.dtype] = None
         self._name: Optional[str] = None
         self._is_complex: bool = False
 
     def __repr__(self):
         return f"TorchScriptTensor('{self._torch_value!r}')"
 
     @property  # type: ignore[override]
@@ -145,23 +147,27 @@
     def shape(self, shape: Tuple[int | None, ...]):
         self._shape = shape
         self._torch_value.setType(self._torch_value.type().with_sizes(list(shape)))
 
     @property  # type: ignore[override]
     def dtype(self) -> torch.dtype | None:
         # TODO: Return numpy dtype
+        if self._torch_dtype is not None:
+            return self._torch_dtype
         torch_dtype = _type_utils.JitScalarType.from_value(  # type: ignore[attr-defined]
             self._torch_value, default=_type_utils.JitScalarType.UNDEFINED
         )
         if torch_dtype == _type_utils.JitScalarType.UNDEFINED:
             return None
-        return torch_dtype.dtype()
+        self._torch_dtype = torch_dtype.dtype()
+        return self._torch_dtype
 
     @dtype.setter
     def dtype(self, dtype: torch.dtype):
+        self._torch_dtype = dtype
         self._torch_value.setType(self._torch_value.type().with_dtype(dtype))
 
     @property
     def is_complex(self) -> bool:
         return self._is_complex
 
     @is_complex.setter
@@ -689,15 +695,19 @@
             dynamic_axes={},
             defer_weight_export=False,
             operator_export_type=torch.onnx.OperatorExportTypes.ONNX,
             strip_doc_string=False,
             keep_initializers_as_inputs=False,
             custom_opsets={},
             add_node_names=True,
-            onnx_file_path="",
+            # TODO(#493): Passing in this instead of reading from env.
+            # User must put the exported model file in the same folder to launch ORT.
+            onnx_file_path=os.path.join(
+                os.getenv("EXTERNAL_ONNX_INITIALIZER_FOLDER", ""), "dummy_model_path.onnx"
+            ),
             node_attr_to_name={},
         )
 
         onnx_model = onnx.load_from_string(proto)
         onnx_model.functions.extend(function_proto_dict.values())
 
         # `_export_onnx` only exports opset_imports that is visible to it. It does not
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/graph_building_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/graph_building_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Test cases for graph building functionality."""
 # mypy: disable-error-code="arg-type,type-arg,valid-type"
 from __future__ import annotations
 
+import os
+import tempfile
 import unittest
 
 import torch
 
 import onnxscript
 import onnxscript.testing
 from onnxscript import FLOAT, evaluator
@@ -135,9 +137,43 @@
     def test_add_initializer_allows_adding_the_same_tensor_twice_using_same_name(self):
         graph = graph_building.TorchScriptGraph()
         x_tensor = torch.ones((1, 2, 3), dtype=torch.float32)
         graph.add_initializer("x", x_tensor)
         graph.add_initializer("x", x_tensor)
 
 
+class TestModelSaving(unittest.TestCase):
+    @unittest.skipIf(os.getenv("CI") == "true", "CI is not ready to run dyanmo_export.")
+    def test_save_initializer_to_files_for_large_model(self):
+        class MLP(torch.nn.Module):
+            def __init__(self, input_size, hidden_size, output_size):
+                super().__init__()
+                self.fc1 = torch.nn.Linear(input_size, hidden_size)
+                self.fc2 = torch.nn.Linear(hidden_size, output_size)
+                self.relu = torch.nn.ReLU()
+
+            def forward(self, x):
+                out = self.fc1(x)
+                out = self.relu(out)
+                out = self.fc2(out)
+                return out
+
+        # # of model parameters:
+        #  input_size x hidden_size + hidden_size +
+        #  hidden_size x output_size + output_size
+        #  ~= 3GB below
+        batch_size, input_size, hidden_size, output_size = 1, 4, 50000000, 10
+        model = MLP(input_size, hidden_size, output_size)
+        x = torch.randn(batch_size, input_size)
+
+        with tempfile.TemporaryDirectory() as temp_dir:
+            os.environ["EXTERNAL_ONNX_INITIALIZER_FOLDER"] = temp_dir
+            torch.onnx.dynamo_export(
+                model,
+                x,
+            )
+            # 3 initializers are saved to files as external data.
+            self.assertEqual(len(os.listdir(temp_dir)), 3)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,27 @@
     we want to delay the compilation of the function.
 """
 from __future__ import annotations
 
 import math
 from typing import Any, Optional, Sequence, Tuple, Union
 
-from onnxscript import BOOL, DOUBLE, FLOAT, INT8, INT16, INT32, INT64, UINT8, graph
+from onnxscript import (
+    BFLOAT16,
+    BOOL,
+    DOUBLE,
+    FLOAT,
+    FLOAT16,
+    INT8,
+    INT16,
+    INT32,
+    INT64,
+    UINT8,
+    graph,
+)
 from onnxscript.function_libs.torch_lib.registration import torch_op
 from onnxscript.function_libs.torch_lib.tensor_typing import (
     IntType,
     RealType,
     TFloat,
     TFloatHighPrecision,
     TFloatOrBFloat16,
@@ -36,19 +48,27 @@
 
 _INT64_MAX = 9223372036854775807
 _INT64_MIN = -9223372036854775808
 _MATH_PI = math.pi
 
 
 @torch_op("aten::_local_scalar_dense")
-def aten__local_scalar_dense(self: TTensor) -> TTensor:
+def aten__local_scalar_dense(self: Union[FLOAT16, FLOAT, DOUBLE, BFLOAT16]) -> FLOAT:
+    """_local_scalar_dense(Tensor self) -> Scalar"""
+
+    # Return the first element in tensor as a scalar.
+    return op.Cast(op.Gather(op.Reshape(self, [-1]), 0), to=FLOAT.dtype)
+
+
+@torch_op("aten::_local_scalar_dense")
+def aten__local_scalar_dense_int(self: IntType) -> INT64:
     """_local_scalar_dense(Tensor self) -> Scalar"""
 
     # Return the first element in tensor as a scalar.
-    return op.Gather(op.Reshape(self, [-1]), 0)
+    return op.Cast(op.Gather(op.Reshape(self, [-1]), 0), to=INT64.dtype)
 
 
 @torch_op("aten::abs")
 def aten_abs(self: TRealOrUInt8) -> TRealOrUInt8:
     """abs(Tensor self) -> Tensor"""
 
     return op.Abs(self)
@@ -242,38 +262,38 @@
     raise NotImplementedError()
 
 
 @torch_op("aten::all")
 def aten_all(self: TTensor) -> BOOL:
     """all(Tensor self) -> Tensor"""
 
-    if op.Size(op.Shape(self)) == 0:
+    self_rank = op.Size(op.Shape(self))
+    if self_rank == 0:
         result = op.Cast(self, to=BOOL.dtype)
     else:
         self_bool = op.Cast(self, to=BOOL.dtype)
         self_int = op.Cast(self_bool, to=INT64.dtype)
-        result_int = op.ReduceMin(self_int, keepdims=0)
-        result = op.Cast(result_int, to=BOOL.dtype)
-
+        all_true = op.ReduceMin(self_int, keepdims=False)
+        result = op.Cast(all_true, to=BOOL.dtype)
     return result
 
 
 @torch_op("aten::all.dim")
 def aten_all_dim(self: TTensor, dim: int, keepdim: bool = False) -> BOOL:
     """all.dim(Tensor self, int dim, bool keepdim=False) -> Tensor"""
 
-    if op.Size(op.Shape(self)) == 0:
+    self_rank = op.Size(op.Shape(self))
+    if self_rank == 0:
         result = op.Cast(self, to=BOOL.dtype)
     else:
         self_bool = op.Cast(self, to=BOOL.dtype)
         self_int = op.Cast(self_bool, to=INT64.dtype)
         dims = op.Reshape(dim, op.Constant(value_ints=[-1]))
-        result_int = op.ReduceMin(self_int, dims, keepdims=keepdim)
-        result = op.Cast(result_int, to=BOOL.dtype)
-
+        all_true = op.ReduceMin(self_int, dims, keepdims=keepdim)
+        result = op.Cast(all_true, to=BOOL.dtype)
     return result
 
 
 @torch_op("aten::allclose")
 def aten_allclose(
     self: TReal,
     other: TReal,
@@ -288,15 +308,15 @@
     left_part = op.Abs(op.Sub(self, other))
     right_part = op.Add(atol, op.Mul(rtol, op.Abs(other)))
     is_close = op.LessOrEqual(left_part, right_part)
     is_close_int = op.Cast(is_close, to=INT8.dtype)
 
     # If min is 0, some elements are not close -> allclose is False
     # If min is 1, all elements are close -> allclose is True
-    return op.Cast(op.ReduceMin(is_close_int, keepdims=0), to=BOOL.dtype)
+    return op.Cast(op.ReduceMin(is_close_int, keepdims=False), to=BOOL.dtype)
 
 
 def aten_alpha_dropout(input: TensorType, p: float, train: bool) -> TensorType:
     """alpha_dropout(Tensor input, float p, bool train) -> Tensor"""
 
     raise NotImplementedError()
 
@@ -334,49 +354,44 @@
 def aten_angle(self: TensorType) -> TensorType:
     """angle(Tensor self) -> Tensor"""
 
     raise NotImplementedError()
 
 
 @torch_op("aten::any")
-def aten_any(
-    self: TTensor,
-    keepdim: bool = True,  # pylint: disable=unused-argument
-) -> BOOL:
+def aten_any(self: TTensor) -> BOOL:
     """any(Tensor self) -> Tensor"""
 
     self_rank = op.Size(op.Shape(self))
     if self_rank == 0:
-        result = op.Not(op.Equal(self, 0.0))
+        result = op.Cast(self, to=BOOL.dtype)
     else:
-        # cannot cast to INT64 because 0.1 will be cast to 0, then convert to false
         self_bool = op.Cast(self, to=BOOL.dtype)
-        # op.ReduceMax() in next step cannot calculate BOOL value, so convert to INT64
+        # op.ReduceMax() in the next step cannot process BOOL inputs, so convert to INT64
         self_int = op.Cast(self_bool, to=INT64.dtype)
-        result_max = op.ReduceMax(self_int, keepdims=0, noop_with_empty_axes=0)
-        result = op.Greater(result_max, op.Constant(value_int=0))
+        any_true = op.ReduceMax(self_int, keepdims=False)
+        result = op.Cast(any_true, to=BOOL.dtype)
     return result
 
 
 @torch_op("aten::any.dim")
-def aten_any_dim(self: TTensor, dim: int, keepdim: bool = True) -> BOOL:
+def aten_any_dim(self: TTensor, dim: int, keepdim: bool = False) -> BOOL:
     """any.dim(Tensor self, int dim, bool keepdim=False) -> Tensor"""
 
     self_rank = op.Size(op.Shape(self))
     if self_rank == 0:
-        result = op.Not(op.Equal(self, 0.0))
+        result = op.Cast(self, to=BOOL.dtype)
     else:
-        # cannot cast to INT64 because 0.1 will be cast to 0, then convert to false
         self_bool = op.Cast(self, to=BOOL.dtype)
-        # op.ReduceMax() in next step cannot calculate BOOL value, so convert to INT64
+        # op.ReduceMax() in the next step cannot process BOOL inputs, so convert to INT64
         self_int = op.Cast(self_bool, to=INT64.dtype)
         # Change dim from int to INT64[1]
         dims = op.Reshape(dim, op.Constant(value_ints=[-1]))
-        result_max = op.ReduceMax(self_int, dims, keepdims=keepdim, noop_with_empty_axes=0)
-        result = op.Greater(result_max, op.Constant(value_int=0))
+        any_true = op.ReduceMax(self_int, dims, keepdims=keepdim)
+        result = op.Cast(any_true, to=BOOL.dtype)
     return result
 
 
 def _range_supported(dtype: int) -> bool:
     """Returns true if the dtype is supported by the ONNX Range op."""
     return dtype in {
         DOUBLE.dtype,
@@ -2048,14 +2063,15 @@
 
 @torch_op("aten::cumsum", trace_only=True)
 def aten_cumsum(
     self: TRealUnlessInt16OrInt8, dim: Union[INT32, INT64], dtype: int = -1
 ) -> TRealUnlessInt16OrInt8:
     """cumsum(Tensor self, int dim, *, ScalarType? dtype=None) -> Tensor"""
 
+    # TODO(justinchuby): The accumulation type for int32 is int64. Consider excluding from inputs.
     if dtype == -1:
         cast = self
     else:
         cast = op.Cast(self, to=dtype)
     return _aten_cumsum_onnx(cast, dim)
 
 
@@ -2360,18 +2376,21 @@
     return op.Equal(self, other)
 
 
 @torch_op("aten::equal")
 def aten_equal(self: TTensor, other: TTensor) -> BOOL:
     """equal(Tensor self, Tensor other) -> bool"""
 
-    sub_self_other = op.Sub(self, other)
-    abs_sub = op.Abs(sub_self_other)
-    sum_of_abs = op.ReduceSum(abs_sub, keepdims=0)
-    return op.Equal(sum_of_abs, 0)
+    # NOTE: Torch aten::equal returns a single Boolean while ONNX Equal is elementwise.
+    # The equivalent Torch op with ONNX Equal is aten::eq.
+    elementwise_equal = op.Equal(self, other)
+    elementwise_equal_int = op.Cast(elementwise_equal, to=INT64.dtype)
+    # ReduceMax does not support bool. So we cast to int64
+    all_equal = op.ReduceMin(elementwise_equal_int, keepdims=False)
+    return op.Cast(all_equal, to=BOOL.dtype)
 
 
 def aten_erfinv(self: TensorType) -> TensorType:
     """erfinv(Tensor self) -> Tensor"""
 
     raise NotImplementedError()
 
@@ -3398,15 +3417,15 @@
     other_rank = op.Size(op.Shape(other))
     result = op.Equal(self_rank, other_rank)
     if result:  # Same rank, then compare shape
         self_shape = op.Shape(self)
         other_shape = op.Shape(other)
         result_bool = op.Equal(self_shape, other_shape)
         result_int = op.Cast(result_bool, to=INT8.dtype)
-        result = op.Cast(op.ReduceMin(result_int, keepdims=0), to=BOOL.dtype)
+        result = op.Cast(op.ReduceMin(result_int, keepdims=False), to=BOOL.dtype)
 
     return result
 
 
 def aten_is_set_to(self: TensorType, tensor: TensorType) -> bool:
     """is_set_to(Tensor self, Tensor tensor) -> bool"""
 
@@ -3634,18 +3653,19 @@
 
 def aten_lift_fresh(self: TensorType) -> TensorType:
     """lift_fresh(Tensor(a) self) -> Tensor(a)"""
 
     raise NotImplementedError()
 
 
+@torch_op("aten::lift_fresh_copy")
 def aten_lift_fresh_copy(self: TensorType) -> TensorType:
     """lift_fresh_copy(Tensor self) -> Tensor"""
 
-    raise NotImplementedError()
+    return op.Identity(self)
 
 
 def aten_linear_backward(
     self: TensorType, grad_output: TensorType, weight: TensorType, output_mask: Sequence[bool]
 ) -> tuple[TensorType, TensorType, TensorType]:
     """linear_backward(Tensor self, Tensor grad_output, Tensor weight, bool[3] output_mask) -> (Tensor, Tensor, Tensor)"""
 
@@ -3729,24 +3749,35 @@
     """logaddexp2(Tensor self, Tensor other) -> Tensor"""
     summation = op.Add(op.Pow(2.0, self), op.Pow(2.0, other))
 
     return op.Div(op.Log(summation), op.Log(2.0))
 
 
 @torch_op("aten::logcumsumexp")
-def aten_logcumsumexp(self: TFloatOrBFloat16, dim: INT64) -> TFloatOrBFloat16:
+def aten_logcumsumexp(self: TFloatOrBFloat16, dim: int) -> TFloatOrBFloat16:
     """logcumsumexp(Tensor self, int dim) -> Tensor"""
 
-    if op.Size(op.Shape(self)) == 0:
-        # A scalar
-        result = op.Identity(self)
+    self_rank = op.Size(op.Shape(self))
+    if self_rank == 0:
+        result = self
     else:
-        # FIXME(justinchuby): Ensure numerical stability
-        result = op.Log(op.CumSum(op.Exp(self), dim))
-
+        # Make dim 1-d
+        dims = op.Unsqueeze(dim, axes=[0])
+        # This uses the max trick to avoid overflow:
+        # Assuming A = [a_1, a_2, ..., a_n] and the output
+        # out = [out_1, out_2, ..., out_n], then
+        # out_i = log(cumsum(exp(A)))_i
+        #       = log(exp(a_1) + ... + exp(a_i))
+        #       = log(exp(a_1) + ... + exp(a_i)) - max(A) + max(A)
+        #       = log((exp(a_1) + ... + exp(a_i)) / exp(max(A))) + max(A)
+        #       = log(exp(a_1-max(A)) + ... + exp(a_i-max(A))) + max(A)
+        #       = log(sum<j=1...i>(exp(a_j - max(A)))) + max(A)
+        # Vectorizing for all i, we get the expression below.
+        self_max = op.ReduceMax(self, dims)
+        result = op.Log(op.CumSum(op.Exp(self - self_max), dims)) + self_max
     return result
 
 
 @torch_op("aten::logdet")
 def aten_logdet(self: TFloat) -> TFloat:
     """logdet(Tensor self) -> Tensor"""
 
@@ -4031,15 +4062,15 @@
 def aten_max(self: TReal) -> TReal:
     """max(Tensor self) -> Tensor"""
 
     self_rank = op.Size(op.Shape(self))
     if self_rank == 0:
         self = op.Reshape(self, op.Constant(value_ints=[-1]))
 
-    result = op.ReduceMax(self, keepdims=0)
+    result = op.ReduceMax(self, keepdims=False)
 
     if self_rank == 0:
         result = op.Squeeze(result)
 
     return result
 
 
@@ -4097,15 +4128,15 @@
     raise NotImplementedError()
 
 
 @torch_op("aten::min")
 def aten_min(self: TReal) -> TReal:
     """min(Tensor self) -> Tensor"""
 
-    return op.ReduceMin(self, keepdims=0)
+    return op.ReduceMin(self, keepdims=False)
 
 
 @torch_op("aten::min.dim")
 def aten_min_dim(self: TReal, dim: int, keepdim: bool = False) -> Tuple[TReal, TInt]:
     """min.dim(Tensor self, int dim, bool keepdim=False) -> (Tensor values, Tensor indices)"""
     if op.Size(op.Shape(self)) == 0:
         result = self
@@ -4654,18 +4685,18 @@
         momentum=momentum,
         training_mode=training,
     )
     # Compute var and rstd
     mean = op.ReduceMean(input, axes)
     input_sub_mean = op.Sub(input, mean)
     sqr = op.Mul(input_sub_mean, input_sub_mean)
-    var = op.ReduceMean(sqr, axes, keepdims=0)
+    var = op.ReduceMean(sqr, axes, keepdims=False)
     rstd = op.Div(1.0, op.Sqrt(var + eps))
     # Get mean again with size = [1, C]
-    mean = op.ReduceMean(input, axes, keepdims=0)
+    mean = op.ReduceMean(input, axes, keepdims=False)
     return norm, mean, rstd
 
 
 @torch_op("aten::native_batch_norm", private=True)
 def _aten_native_batch_norm_inference_onnx(
     input: TFloat,
     weight: TFloat,
@@ -4803,18 +4834,18 @@
     # The output size is [N, group], so dims = [2]
     axes = op.Constant(value_ints=[2])
     # Get mean which size is [N, group, 1], for broadcasting
     mean = op.ReduceMean(input_N_group_neg1, axes)
     input_sub_mean = op.Sub(input_N_group_neg1, mean)
     sqr_input_sub_mean = op.Mul(input_sub_mean, input_sub_mean)
     # In Pytorch, vstd = 1/(sqrt(var + eps))
-    var = op.ReduceMean(sqr_input_sub_mean, axes, keepdims=0)
+    var = op.ReduceMean(sqr_input_sub_mean, axes, keepdims=False)
     rstd = op.Div(1.0, op.Sqrt(var + eps))
     # Get the correct shape [N, group] for mean again
-    mean = op.ReduceMean(input_N_group_neg1, axes, keepdims=0)
+    mean = op.ReduceMean(input_N_group_neg1, axes, keepdims=False)
     return norm_result, mean, rstd
 
 
 def aten_native_group_norm_backward(
     grad_out: TensorType,
     input: TensorType,
     mean: TensorType,
@@ -5016,16 +5047,17 @@
 
     raise NotImplementedError()
 
 
 @torch_op("aten::nonzero")
 def aten_nonzero(self: TTensor) -> INT64:
     """nonzero(Tensor self) -> Tensor"""
-
-    return op.NonZero(self)
+    # NOTE: In torch the return shape is [n, d], while in onnx [d, n],
+    # where `d` is rank of input tensor, `n` is number of nonzero elements.
+    return op.Transpose(op.NonZero(self), perm=[1, 0])
 
 
 def aten_nonzero_numpy(self: TensorType) -> TensorType:
     """nonzero_numpy(Tensor self) -> Tensor[]"""
 
     raise NotImplementedError()
 
@@ -5688,20 +5720,74 @@
     b_hh: Optional[TensorType] = None,
 ) -> TensorType:
     """rnn_tanh_cell(Tensor input, Tensor hx, Tensor w_ih, Tensor w_hh, Tensor? b_ih=None, Tensor? b_hh=None) -> Tensor"""
 
     raise NotImplementedError()
 
 
-def aten_roll(
-    self: TensorType, shifts: Sequence[int], dims: Optional[Sequence[int]] = None
-) -> TensorType:
+@torch_op("aten::roll", trace_only=True)
+def aten_roll(self: TTensor, shifts: INT64, dims: Sequence[int] = ()) -> TTensor:
     """roll(Tensor self, int[1] shifts, int[1] dims=[]) -> Tensor"""
 
-    raise NotImplementedError()
+    self_rank = len(self.shape)
+    if self_rank == 0:
+        return self
+    elif self.shape[0] == 0:  # empty tensor
+        return self
+    else:
+        if isinstance(dims, tuple) and len(dims) == 0:  # Empty list
+            # assert isinstance(shifts, int)
+            return _aten_roll_shift_no_dim_onnx(self, shifts)
+        else:
+            # assert len(shifts) == len(dims), but shifts is a tensor, dims is a list
+            result = self
+            for i in range(len(shifts)):  # pylint: disable=consider-using-enumerate
+                shift = op.Gather(shifts, i, axis=0)
+                dim = dims[i]
+                result = _aten_roll_shift_and_dim_onnx(result, shift, dim)
+            return result
+
+
+@torch_op("aten::roll", private=True)
+def _aten_roll_shift_no_dim_onnx(self: TTensor, shift: INT64) -> TTensor:
+    neg_1 = op.Constant(value_ints=[-1])
+    # flatten the self tensor: from [[A,B],[C,D]] to [A,B,C,D]
+    self_flatten = op.Reshape(self, neg_1)
+    # Compute slice length
+    shift_tensor = op.Reshape(shift, neg_1)
+    if shift_tensor < 0:
+        # For [A,B,C,D], if shift is -1, slice_length = -(-1) = 1, means move [A] to the end
+        slice_length = -shift_tensor
+    else:
+        # For [A,B,C,D], if shift is 1, slice_length = 4 - 1 = 3, means move [A,B,C] to the end
+        # The effect equals to move [D] to the beginning
+        slice_length = op.Size(self_flatten) - shift_tensor
+    # Get second part of the tensor, e.g. [A,B,C]
+    suffix = op.Slice(self_flatten, op.Constant(value_ints=[0]), slice_length)
+    # Get first part of the tensor, e.g. [D]
+    prefix = op.Slice(self_flatten, slice_length, op.Reshape(op.Size(self_flatten), neg_1))
+    # Concat first+second together, e.g. [D,A,B,C]
+    result = op.Concat(prefix, suffix, axis=0)
+    return op.Reshape(result, op.Shape(self))
+
+
+@torch_op("aten::roll", private=True)
+def _aten_roll_shift_and_dim_onnx(self: TTensor, shift: INT64, dim: int) -> TTensor:
+    neg_1 = op.Constant(value_ints=[-1])
+    dim_tensor = op.Reshape(op.Constant(value_int=dim), neg_1)
+    shift_tensor = op.Reshape(shift, neg_1)
+    if shift_tensor < 0:
+        slice_length = -shift_tensor
+    else:
+        slice_length = op.Gather(op.Shape(self), dim_tensor, axis=0) - shift_tensor
+    # from [A,B,C,D] -> [D,A,B,C], [D] is prefix, [A,B,C] is suffix
+    suffix = op.Slice(self, op.Constant(value_ints=[0]), slice_length, axes=dim_tensor)
+    prefix = op.Slice(self, slice_length, op.Reshape(op.Size(self), neg_1), axes=dim_tensor)
+    result = op.Concat(prefix, suffix, axis=dim)
+    return result
 
 
 def aten_rot90(self: TensorType, k: int = 1, dims: Sequence[int] = (0, 1)) -> TensorType:
     """rot90(Tensor self, int k=1, int[] dims=[0,1]) -> Tensor"""
 
     raise NotImplementedError()
 
@@ -5768,14 +5854,23 @@
 @torch_op("aten::scalar_tensor")
 def aten_scalar_tensor(s: float, dtype: int = FLOAT.dtype) -> TTensor:  # type: ignore[type-var]
     """scalar_tensor(Scalar s, *, ScalarType? dtype=None, Layout? layout=None, Device? device=None, bool? pin_memory=None) -> Tensor"""
 
     return op.Cast(s, to=dtype)
 
 
+@torch_op("aten::scalar_tensor")
+def aten_scalar_tensor_sym_number(
+    s: Union[FLOAT, INT32, BOOL], dtype: int = FLOAT.dtype
+) -> TTensor:
+    """scalar_tensor(Scalar s, *, ScalarType? dtype=None, Layout? layout=None, Device? device=None, bool? pin_memory=None) -> Tensor"""
+
+    return op.Cast(s, to=dtype)
+
+
 @torch_op("aten::scatter_add")
 def aten_scatter_add(
     self: TReal,
     dim: int,  # we have to use int here because ScatterElements() will use this attribute
     index: TInt,
     src: TReal,
 ) -> TReal:
@@ -6730,15 +6825,15 @@
 
 
 @torch_op(("aten::unbind", "aten::unbind.int"))
 def aten_unbind(self: TTensor, dim: int = 0) -> Sequence[TTensor]:
     """unbind.int(Tensor(a -> *) self, int dim=0) -> Tensor(a)[]"""
 
     split_sizes = op.Constant(value_int=1)
-    return op.SplitToSequence(self, split_sizes, axis=dim, keepdims=0)
+    return op.SplitToSequence(self, split_sizes, axis=dim, keepdims=False)
 
 
 @torch_op("aten::unflatten")
 def aten_unflatten(self: TReal, dim: INT64, sizes: INT64):
     """unflatten(Tensor(a) self, int dim, SymInt[] sizes) -> Tensor(a)"""
 
     self_size = op.Shape(self)
@@ -6974,37 +7069,37 @@
     mean = op.ReduceMean(self, keepdims=keepdim)
     sub_mean = op.Sub(self, mean)
     sqr_mean = op.Mul(sub_mean, sub_mean)
     var = op.ReduceMean(sqr_mean, keepdims=keepdim)
     # Adjust var according to correction value
     if correction > 0.0:
         self_shape = op.Shape(self)
-        numel_float = op.Cast(op.ReduceProd(self_shape, keepdims=0), to=FLOAT.dtype)
+        numel_float = op.Cast(op.ReduceProd(self_shape, keepdims=False), to=FLOAT.dtype)
         mul = op.Mul(var, numel_float)
         sub = op.Sub(numel_float, correction)
         var = op.Div(mul, sub)
 
     return var, mean
 
 
 @torch_op("aten::var_mean.dim", private=True)
 def _aten_var_mean_dim_onnx(
     self: TReal, dim: INT64, correction: float, keepdim: bool = False
 ) -> Tuple[TReal, TReal]:
     dim = op.Reshape(dim, op.Constant(value_ints=[-1]))
     # Computer mean and var
     mean = op.ReduceMean(self, dim, keepdims=keepdim)
-    sub_mean = op.Sub(self, op.ReduceMean(self, dim, keepdims=1))
+    sub_mean = op.Sub(self, op.ReduceMean(self, dim, keepdims=True))
     sqr_mean = op.Mul(sub_mean, sub_mean)
     var = op.ReduceMean(sqr_mean, dim, keepdims=keepdim)
     # Adjust var according to correction value
     if correction > 0.0:
         self_shape = op.Shape(self)
         dim_size = op.Gather(self_shape, dim, axis=0)
-        numel_float = op.CastLike(op.ReduceProd(dim_size, keepdims=0), self)
+        numel_float = op.CastLike(op.ReduceProd(dim_size, keepdims=False), self)
         mul = op.Mul(var, numel_float)
         sub = op.Sub(numel_float, correction)
         var = op.Div(mul, sub)
 
     return var, mean
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1140,17 +1140,17 @@
 
 @torch_op("aten::mse_loss")
 def aten_mse_loss(self: TReal, target: TReal, reduction: int = 1) -> TReal:
     """mse_loss(Tensor self, Tensor target, int reduction=Mean) -> Tensor"""
     # FIXME: When reduction=0, the shape(result) will be different than other case
     result = op.Mul(self - target, self - target)
     if reduction == 1:  # mean
-        result = op.ReduceMean(result, keepdims=0)
+        result = op.ReduceMean(result, keepdims=False)
     if reduction == 2:  # sum
-        result = op.ReduceSum(result, keepdims=0)
+        result = op.ReduceSum(result, keepdims=False)
 
     return result
 
 
 def aten_mse_loss_backward(
     grad_output: TensorType, self: TensorType, target: TensorType, reduction: int
 ) -> TensorType:
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 from __future__ import annotations
 
 from typing import Optional, Sequence
 
 from onnxscript import FLOAT
 from onnxscript.function_libs.torch_lib.registration import torch_op
-from onnxscript.function_libs.torch_lib.tensor_typing import TFloatOrBFloat16, TReal
+from onnxscript.function_libs.torch_lib.tensor_typing import TFloatOrBFloat16
 from onnxscript.onnx_opset import opset18 as op
 from onnxscript.onnx_types import TensorType
 
 
 def aten_special_airy_ai(x: TensorType) -> TensorType:
     """special_airy_ai(Tensor x) -> Tensor"""
 
@@ -83,22 +83,22 @@
 def aten_special_entr(self: TensorType) -> TensorType:
     """special_entr(Tensor self) -> Tensor"""
 
     raise NotImplementedError()
 
 
 @torch_op(("aten::erf", "aten::special_erf"))
-def aten_special_erf(self: TReal) -> TReal:
+def aten_special_erf(self: TFloatOrBFloat16) -> TFloatOrBFloat16:
     """erf(Tensor self) -> Tensor"""
 
     return op.Erf(self)
 
 
 @torch_op(("aten::erfc", "aten::special_erfc"))
-def aten_special_erfc(self: TReal) -> TReal:
+def aten_special_erfc(self: TFloatOrBFloat16) -> TFloatOrBFloat16:
     """erfc(Tensor self) -> Tensor"""
 
     return op.Sub(1, op.Erf(self))
 
 
 @torch_op("aten::special_erfcx")
 def aten_special_erfcx(self: TFloatOrBFloat16) -> TFloatOrBFloat16:
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/irbuilder.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/irbuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,16 +519,16 @@
     ) -> None:
         fn.add_attr_parameter(IRAttributeParameter(varname, attribute_type, default_value))
 
     def add_output(self, fn: IRFunction, varname: str, typeinfo, sourceinfo) -> None:
         var = IRVar(varname, typeinfo, sourceinfo)
         fn.append_output(var)
 
-    def make_attr(self, attrname: str, attrval: Any) -> IRAttributeValue:
-        return IRAttributeValue(helper.make_attribute(attrname, attrval))
+    def make_attr(self, attrproto: onnx.AttributeProto) -> IRAttributeValue:
+        return IRAttributeValue(attrproto)
 
     def make_attr_ref(self, attrname: str, refname: str, pytype: type) -> IRAttributeValue:
         proto = onnx.AttributeProto()
         proto.name = attrname
         proto.ref_attr_name = refname
         attr_type = ta.pytype_to_attrtype(pytype)
         assert attr_type is not None
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/main.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/__init__.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_types.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/sourceinfo.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tensor.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 from typing import Any, Optional
 
 import numpy as np
 import onnx.helper
 from onnx import TensorProto
 
-from onnxscript import autocast, onnx_opset
+from onnxscript import onnx_opset
+from onnxscript._internal import autocast
 
 
 class Tensor:
     """An implementation of ONNX Tensors, based on a wrapper around numpy arrays.
     Serves to define overloaded ops with an ONNX/ONNXScript semantics.
     """
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tensor_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tensor_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/testing.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/testing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/common/onnx_script_test_case.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/common/onnx_script_test_case.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/eager_mode_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/eager_mode_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/eager_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/eager_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/external_tensor_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/external_tensor_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/function_libs/torch_lib/ops_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,22 +35,20 @@
 # complex64 will be flattened to float32.
 TESTED_DTYPES = (
     torch.float16,
     torch.float32,
     # Uncomment below item when we really need testing it
     # torch.bfloat16,
     # torch.float64,
-    # torch.bool,
+    torch.bool,
     # torch.int8,
     # torch.int16,
-    # torch.int32,
+    torch.int32,
     torch.int64,
     # torch.uint8,
-    # torch.complex64,
-    # ......
 )
 # NOTE: torch.complex32 is experimental in torch
 COMPLEX_TYPES = (torch.complex64,)
 
 
 def dtypes_except(*dtypes: torch.dtype) -> Sequence[torch.dtype]:
     """Returns all dtypes except the ones specified."""
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test_common.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/function_libs/torch_lib/ops_test_common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test_data.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/function_libs/torch_lib/ops_test_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -316,14 +316,22 @@
         # aten_nll_loss can only accept integer argument instead of string
         reduction_vals = ["none", "mean", "sum"]
         value = kwargs["reduction"]
         kwargs["reduction"] = reduction_vals.index(value)
     return args, kwargs
 
 
+def _nonzero_input_wrangler(
+    args: list[Any], kwargs: dict[str, Any]
+) -> tuple[list[Any], dict[str, Any]]:
+    if "as_tuple" in kwargs:
+        del kwargs["as_tuple"]
+    return args, kwargs
+
+
 def _randn_input_wrangler(
     args: list[Any], kwargs: dict[str, Any]
 ) -> tuple[list[Any], dict[str, Any]]:
     # Make the size argument as attribute list[int]
     kwargs["size"] = args.pop(0).tolist()
     return args, kwargs
 
@@ -355,14 +363,40 @@
 def _replication_pad3d_input_wrangler(
     args: list[Any], kwargs: dict[str, Any]
 ) -> tuple[list[Any], dict[str, Any]]:
     args.pop(2)  # remove 'replicate' arg
     return args, kwargs
 
 
+def _roll_input_wrangler(
+    args: list[Any], kwargs: dict[str, Any]
+) -> tuple[list[Any], dict[str, Any]]:
+    if len(args) >= 3:
+        if isinstance(args[2], np.ndarray):  # convert dims to list[int]
+            # Change dims from args to kwargs to keep tuple/list type
+            dims = args.pop(2)
+            kwargs["dims"] = dims.tolist()
+        elif isinstance(args[2], int):  # convert dims to list[int]
+            dims = args.pop(2)
+            kwargs["dims"] = []
+            kwargs["dims"].append(dims)
+    if len(args) >= 2:
+        if isinstance(args[1], int):  # convert shift to tensor
+            args[1] = np.array([args[1]], dtype=np.int64)
+    return args, kwargs
+
+
+def _scalar_tensor_input_wrangler(
+    args: list[Any], kwargs: dict[str, Any]
+) -> tuple[list[Any], dict[str, Any]]:
+    if "requires_grad" in kwargs:
+        del kwargs["requires_grad"]
+    return args, kwargs
+
+
 def _scatter_reduce_input_wrangler(
     args: list[Any], kwargs: dict[str, Any]
 ) -> tuple[list[Any], dict[str, Any]]:
     # Put the string into kwargs, otherwise FullGraph mode could not find get 'reduce' argument
     kwargs["reduce"] = args.pop(4)
     return args, kwargs
 
@@ -527,17 +561,22 @@
         matcher=lambda sample: sample.input[0].equal(torch.tensor([])),
         reason="fixme: ORT aborts with zero-dim tensors. https://github.com/microsoft/onnxruntime/issues/16619",
     ),
     TorchLibOpInfo("ceil", core_ops.aten_ceil),
     TorchLibOpInfo(
         "chunk",
         core_ops.aten_chunk,
-    ).xfail(
-        dtypes=[torch.float16],
+    )
+    .xfail(
+        dtypes=(torch.float16,),
         reason="fixme: SplitToSequence op inference failed. https://github.com/microsoft/onnxruntime/issues/16006",
+    )
+    .xfail(
+        dtypes=(torch.bool,),
+        reason="fixme: ORT does not implement SplitToSequence for bool inputs: https://github.com/microsoft/onnxruntime/issues/16905",
     ),
     TorchLibOpInfo("clamp_max", core_ops.aten_clamp_max).skip(
         enabled_if=ops_test_common.IS_WINDOWS,
         reason="fixme: ORT has memory errors. https://github.com/microsoft/onnxruntime/issues/16492",
     ),
     TorchLibOpInfo("clamp_min", core_ops.aten_clamp_min).skip(
         enabled_if=ops_test_common.IS_WINDOWS,
@@ -577,23 +616,17 @@
     # TorchLibOpInfo("empty_strided", core_ops.aten_empty_strided),  # empty_strided is not in OPS_DB
     TorchLibOpInfo("eq", core_ops.aten_eq),
     TorchLibOpInfo("equal", core_ops.aten_equal),
     TorchLibOpInfo("exp", core_ops.aten_exp),
     TorchLibOpInfo("exp2", core_ops.aten_exp2),
     TorchLibOpInfo("expand", core_ops.aten_expand),
     TorchLibOpInfo("expand_as", core_ops.aten_expand_as),
-    TorchLibOpInfo("erf", special_ops.aten_special_erf).xfail(
-        dtypes=(torch.int64,),
-        reason="fixme: ORT did not implement Erf for int64. https://github.com/microsoft/onnxruntime/issues/16654",
-    ),
+    TorchLibOpInfo("erf", special_ops.aten_special_erf),
     TorchLibOpInfo(
         "erfc", special_ops.aten_special_erfc, tolerance={torch.float16: (1e-2, 2e-4)}
-    ).xfail(
-        dtypes=(torch.int64,),
-        reason="fixme: ORT did not implement Erf for int64. https://github.com/microsoft/onnxruntime/issues/16654",
     ),
     # TorchLibOpInfo("erfcx", special_ops.aten_special_erfcx),  # not in OPS_DB
     TorchLibOpInfo("fill", core_ops.aten_fill),
     TorchLibOpInfo("flip", core_ops.aten_flip, input_wrangler=_flip_input_wrangler),
     TorchLibOpInfo("floor", core_ops.aten_floor),
     TorchLibOpInfo("fmod", core_ops.aten_fmod),
     TorchLibOpInfo("full", core_ops.aten_full),
@@ -636,81 +669,83 @@
     TorchLibOpInfo("index_select", core_ops.aten_index_select),
     TorchLibOpInfo("isclose", core_ops.aten_isclose),
     TorchLibOpInfo("isfinite", core_ops.aten_isfinite),
     TorchLibOpInfo("isinf", core_ops.aten_isinf),
     TorchLibOpInfo("isnan", core_ops.aten_isnan),
     TorchLibOpInfo("isneginf", core_ops.aten_isneginf),
     TorchLibOpInfo("isposinf", core_ops.aten_isposinf),
+    TorchLibOpInfo("lift_fresh_copy", core_ops.aten_lift_fresh_copy),
     TorchLibOpInfo(
         "linalg.vector_norm",
         linalg_ops.aten_linalg_vector_norm,
         trace_only=True,
         tolerance={torch.float16: (2e-3, 2e-3)},
         input_wrangler=_linalg_vector_norm_input_wrangler,
     ).skip(
         matcher=lambda sample: sample.kwargs.get("ord") == 6,
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="ORT returns a more accurate value for float16 with ord=6 (expected=Inf, actual=9.48).",
     ),
     TorchLibOpInfo(
         "linspace",
         core_ops.aten_linspace,
         trace_only=True,
     )
     .xfail(
-        dtypes=(torch.int64,),
+        dtypes=(torch.int64, torch.int32),
         reason="fixme: Results do not match with PyTorch. https://github.com/microsoft/onnxscript/issues/854",
     )
     .xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="op 'Range' doesn't support float16.",
     )
     .skip(
         matcher=lambda sample: len(sample.args) > 1 and sample.args[1] == 1,
         reason="aten::linspace with steps=1 is not supported by its definition.",
     ),
     TorchLibOpInfo("log", core_ops.aten_log),
     TorchLibOpInfo("le", core_ops.aten_le),
     TorchLibOpInfo(
         "log10",
         core_ops.aten_log10,
     ).xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: Shape inference error(s): (op_type:Div, node name: n3): B has inconsistent type tensor(float).",
     ),
     TorchLibOpInfo("log1p", core_ops.aten_log1p),
     TorchLibOpInfo(
         "log_softmax",
         special_ops.aten_special_log_softmax,
         tolerance={torch.float32: (3.7e-5, 1.8e-4), torch.float16: (4e-4, 6e-3)},
     ).xfail(
         variant_name="with_dtype",
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: ORT failed. https://github.com/microsoft/onnxruntime/issues/16438",
         test_class_name="TestOutputConsistencyFullGraph",
     ),
     TorchLibOpInfo(
         "log2",
         core_ops.aten_log2,
     ).xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: RuntimeError: Unable to create onnxruntime InferenceSession for executing .Div op with onnx model",
     ),
     TorchLibOpInfo("logaddexp", core_ops.aten_logaddexp),
     TorchLibOpInfo("logaddexp2", core_ops.aten_logaddexp2),
-    TorchLibOpInfo("logcumsumexp", core_ops.aten_logcumsumexp).xfail(
-        reason="naive implementation not numerically stable"
-    ),
+    TorchLibOpInfo("logcumsumexp", core_ops.aten_logcumsumexp),
     TorchLibOpInfo("logdet", core_ops.aten_logdet),
     TorchLibOpInfo(
         "logsumexp",
         core_ops.aten_logsumexp,
     ),
     TorchLibOpInfo("lt", core_ops.aten_lt),
-    TorchLibOpInfo("masked_fill", core_ops.aten_masked_fill),
+    TorchLibOpInfo("masked_fill", core_ops.aten_masked_fill).xfail(
+        dtypes=(torch.bool,),
+        reason="fixme: ORT does not have an implementation for Where with bool inputs.",
+    ),
     TorchLibOpInfo(
         "matmul",
         core_ops.aten_matmul,
         tolerance={torch.float32: (2e-5, 2e-5)},  # Windows requires a more relaxed tolerance
     ).skip(
         matcher=lambda sample: torch.numel(sample.input) == 0,
         reason="values of matmul of [m, 0] and [0, n] matrices are undefined",
@@ -871,15 +906,15 @@
         nn_ops.aten_adaptive_avg_pool3d,
     )
     .xfail(
         matcher=lambda sample: sample.args[0] != (1, 1, 1),
         reason="only global pooling is supported; only batched inputs are supported",
     )
     .xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: RuntimeError: ORT inference error GlobalAveragePool",
     ),
     TorchLibOpInfo("nn.functional.celu", nn_ops.aten_celu),
     TorchLibOpInfo(
         "nn.functional.cross_entropy",
         # use cross_entropy as test case instead of cross_entropy_loss (not in OPS_DB)
         nn_ops.aten_cross_entropy_loss,
@@ -897,15 +932,15 @@
         matcher=lambda sample: len(sample.kwargs) == 0 or sample.kwargs.get("p", 0.0) > 0.0,
         reason="dropout is random so the result not match",
     ),
     TorchLibOpInfo(
         "nn.functional.elu",
         nn_ops.aten_elu,
     ).skip(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: ONNX Runtime aborted",
     ),
     TorchLibOpInfo(
         "nn.functional.embedding",
         core_ops.aten_embedding,
         input_wrangler=_embedding_input_wrangler,
     ),
@@ -974,47 +1009,53 @@
         ),
         reason="this Aten overload need args[1] == 'replicate' for pad mode, and 3D tensor",
     ),
     TorchLibOpInfo(
         "nn.functional.selu",
         core_ops.aten_selu,
     ).skip(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: ONNX Runtime aborted",
     ),
     TorchLibOpInfo(
         "nn.functional.mse_loss",
         nn_ops.aten_mse_loss,
         input_wrangler=_mse_loss_input_wrangler,
     ),
     TorchLibOpInfo(
         "nonzero",
         core_ops.aten_nonzero,
-    ).xfail(
-        matcher=lambda sample: sample.kwargs.get("as_tuple") is not None,
+        input_wrangler=_nonzero_input_wrangler,
+    )
+    .xfail(
+        matcher=lambda sample: sample.kwargs.get("as_tuple"),
         reason="as_tuple=True is not supported",
+    )
+    .xfail(
+        matcher=lambda sample: len(sample.input.shape) == 0,
+        reason="fixme: output 'shape' do not match: torch.Size([0, 1]) != torch.Size([0, 0]).",
     ),
     TorchLibOpInfo(
         "normal",
         core_ops.aten_normal,
         nondeterministic=True,
     )
     .skip(
         matcher=lambda sample: len(sample.args) > 0 and not isinstance(sample.args[0], float),
         reason="ORT only accept float type for args[0] 'mean'",
     )
     .xfail(
         reason="ORT fails on a cast node it inserts for float16. https://github.com/microsoft/onnxruntime/issues/16449",
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         test_class_name="TestOutputConsistencyEager",
     )
     .xfail(
         variant_name="number_mean",
         reason="ORT fails on a cast node it inserts for float16. https://github.com/microsoft/onnxruntime/issues/16449",
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         test_class_name="TestOutputConsistencyEager",
     ),
     TorchLibOpInfo("ones", core_ops.aten_ones),
     TorchLibOpInfo(
         "permute",
         core_ops.aten_permute,
         input_wrangler=_permute_input_wrangler,
@@ -1031,23 +1072,23 @@
     # TorchLibOpInfo("rand", core_ops.aten_rand),  # no test case in OPS_DB
     TorchLibOpInfo(
         "randn",
         core_ops.aten_randn,
         input_wrangler=_randn_input_wrangler,
         nondeterministic=True,
     ).xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: Shape inference error",
     ),
     TorchLibOpInfo("reciprocal", core_ops.aten_reciprocal),
     TorchLibOpInfo(
         "remainder",
         core_ops.aten_remainder,
     ).xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="Eager mode failed on case(self=7.75,other=0.1582) due to precision loss",
         test_class_name="TestOutputConsistencyEager",
     ),
     TorchLibOpInfo("repeat", core_ops.aten_repeat),
     TorchLibOpInfo("reshape", core_ops.aten_reshape),
     TorchLibOpInfo("resolve_conj", core_ops.aten_resolve_conj),
     TorchLibOpInfo("resolve_neg", core_ops.aten_resolve_neg),
@@ -1066,67 +1107,85 @@
     )
     .xfail(
         variant_name="decimals_neg_3",
         reason="The op does not support decimals yet",
     ),
     TorchLibOpInfo("rsqrt", core_ops.aten_rsqrt),
     TorchLibOpInfo("rsub", core_ops.aten_rsub),
-    # TorchLibOpInfo("scalar_tensor", core_ops.aten_scalar_tensor),  # no test case in OPS_DB
+    TorchLibOpInfo(
+        "scalar_tensor",
+        core_ops.aten_scalar_tensor,
+        input_wrangler=_scalar_tensor_input_wrangler,
+    ),
     TorchLibOpInfo(
         "scatter_add",
         core_ops.aten_scatter_add,
     )
     .xfail(
         matcher=lambda sample: len(sample.input.shape) == 0,
         reason="fixme: Rank(0) input will lead ORT failed due to different rank(result) in if-else branch",
     )
     .xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: ORT failed",
     ),
     TorchLibOpInfo("select", core_ops.aten_select),
     TorchLibOpInfo("select_scatter", core_ops.aten_select_scatter),
     TorchLibOpInfo("sigmoid", core_ops.aten_sigmoid),
     TorchLibOpInfo("sign", core_ops.aten_sign),
     TorchLibOpInfo("sin", core_ops.aten_sin),
     TorchLibOpInfo("sinh", core_ops.aten_sinh),
     TorchLibOpInfo(
         "softmax",
         special_ops.aten_special_softmax,
         tolerance={torch.float32: (3.7e-5, 1.8e-4), torch.float16: (3e-4, 4e-4)},
     )
     .xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: ORT failed",
     )
     .xfail(
         variant_name="with_dtype",
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: ORT failed. https://github.com/microsoft/onnxruntime/issues/16438",
         test_class_name="TestOutputConsistencyFullGraph",
     ),
     TorchLibOpInfo(
         "split_with_sizes",
         core_ops.aten_split_with_sizes,
-    ).xfail(
-        dtypes=[torch.float16],
-        reason="fixme: ORT failed",
+    )
+    .xfail(
+        dtypes=(torch.float16,),
+        reason="fixme: ORT failed to produce the correct argument type: https://github.com/microsoft/onnxruntime/issues/16006",
+    )
+    .xfail(
+        dtypes=(torch.bool,),
+        reason="fixme: ORT does not implement SplitToSequence for bool inputs: https://github.com/microsoft/onnxruntime/issues/16905",
     ),
     TorchLibOpInfo(
         "split",
         core_ops.aten_split,
     )
     .xfail(
-        dtypes=[torch.float16],
-        reason="fixme: ORT failed",
+        dtypes=(torch.float16,),
+        reason="fixme: ORT failed to produce the correct argument type: https://github.com/microsoft/onnxruntime/issues/16006",
     )
     .xfail(
         variant_name="list_args",
-        dtypes=[torch.float16],
-        reason="fixme: ORT: Type (seq(tensor(float16))) of output arg (output0) of node () does not match expected type (seq(tensor(float)))",
+        dtypes=(torch.float16,),
+        reason="fixme: ORT failed to produce the correct argument type: https://github.com/microsoft/onnxruntime/issues/16006",
+    )
+    .xfail(
+        dtypes=(torch.bool,),
+        reason="fixme: ORT does not implement SplitToSequence for bool inputs: https://github.com/microsoft/onnxruntime/issues/16905",
+    )
+    .xfail(
+        variant_name="list_args",
+        dtypes=(torch.bool,),
+        reason="fixme: ORT does not implement SplitToSequence for bool inputs: https://github.com/microsoft/onnxruntime/issues/16905",
     ),
     TorchLibOpInfo("sqrt", core_ops.aten_sqrt),
     TorchLibOpInfo(
         "squeeze_dim",
         core_ops.aten_squeeze_dim,
     ).skip(
         matcher=lambda sample: not (len(sample.args) > 0 and isinstance(sample.args[0], int)),
@@ -1156,27 +1215,38 @@
         core_ops.aten_tile,
     ).skip(
         matcher=lambda sample: any(dim == 0 for dim in sample.input.shape)
         or not sample.input.shape,
         reason="fixme: Logic not implemented for size 0 inputs in op.Reshape",
     ),
     TorchLibOpInfo("topk", core_ops.aten_topk).xfail(
-        dtypes=(torch.int64,),
+        dtypes=(torch.int64, torch.int32),
         enabled_if=not ops_test_common.IS_WINDOWS,
         reason="fixme: result mismatch. https://github.com/microsoft/onnxscript/issues/853",
     ),
-    TorchLibOpInfo("tril", core_ops.aten_tril),
-    TorchLibOpInfo("triu", core_ops.aten_triu),
+    TorchLibOpInfo("tril", core_ops.aten_tril).xfail(
+        dtypes=(torch.int32, torch.bool),
+        reason="fixme: ORT does not have an implementation of Trilu for int32 or bool.",
+    ),
+    TorchLibOpInfo("triu", core_ops.aten_triu).xfail(
+        dtypes=(torch.int32, torch.bool),
+        reason="fixme: ORT does not have an implementation of Trilu for int32 or bool.",
+    ),
     TorchLibOpInfo("trunc", core_ops.aten_trunc),
     TorchLibOpInfo(
         "unbind",
         core_ops.aten_unbind,
-    ).xfail(
-        dtypes=[torch.float16],
+    )
+    .xfail(
+        dtypes=(torch.float16,),
         reason="fixme: SplitToSequence op inference failed. https://github.com/microsoft/onnxruntime/issues/16006",
+    )
+    .xfail(
+        dtypes=(torch.bool,),
+        reason="fixme: ORT does not implement SplitToSequence for bool inputs: https://github.com/microsoft/onnxruntime/issues/16905",
     ),
     TorchLibOpInfo(
         "unflatten",
         core_ops.aten_unflatten,
         input_wrangler=_unflatten_input_wrangler,
     )
     .xfail(
@@ -1198,38 +1268,46 @@
     TorchLibOpInfo("view_copy", core_ops.aten_view_copy),
     TorchLibOpInfo(
         "vstack",
         core_ops.aten_vstack,
     ).xfail(
         reason="fixme: A bug of constant-propagation optimization within the subgraph, we can avoid it by turning off graph-optimizations in session options",
     ),
-    TorchLibOpInfo("where", core_ops.aten_where, input_wrangler=_where_input_wrangler),
+    TorchLibOpInfo("where", core_ops.aten_where, input_wrangler=_where_input_wrangler).xfail(
+        dtypes=(torch.bool,),
+        reason="fixme: ORT does not have an implementation for Where with bool inputs.",
+    ),
     TorchLibOpInfo("xlogy", special_ops.aten_special_xlogy),
     TorchLibOpInfo("zeros", core_ops.aten_zeros),
     TorchLibOpInfo(
         "arange_start_step",
         core_ops.aten_arange_start_step,
         trace_only=True,
-    ).xfail(
+    )
+    .xfail(dtypes=(torch.int32,), reason="fixme: output shape mismatch in edge cases.")
+    .xfail(
         matcher=lambda sample: len(sample.args) != 2,
         reason="arange_start_step overload takes three arguments (input, start, step)",
     ),
     TorchLibOpInfo(
         "arange_start",
         core_ops.aten_arange_start,
         trace_only=True,
-    ).skip(
+    )
+    .xfail(dtypes=(torch.int32,), reason="fixme: output shape mismatch in edge cases.")
+    .skip(
         matcher=lambda sample: len(sample.args) != 1,
         reason="arange_start overload takes two arguments (input, start)",
     ),
     TorchLibOpInfo(
         "arange",
         core_ops.aten_arange,
         trace_only=True,
     )
+    .xfail(dtypes=(torch.int32,), reason="fixme: output shape mismatch in edge cases.")
     .xfail(
         matcher=lambda sample: len(sample.args) != 0,
         reason="arange overload takes single argument",
     )
     .xfail(
         matcher=lambda sample: sample.kwargs.get("end") is not None,
         reason="arange overload does not support positional 'end' argument",
@@ -1299,18 +1377,21 @@
         reason="fixme: ORT has memory errors. https://github.com/microsoft/onnxruntime/issues/16492",
     ),
     TorchLibOpInfo(
         "ops.aten.col2im",
         nn_ops.aten_col2im,
         trace_only=True,
     ).xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: Tensor-likes are not close. https://github.com/microsoft/onnxruntime/issues/16007",
     ),
-    TorchLibOpInfo("cumsum", core_ops.aten_cumsum, trace_only=True),
+    TorchLibOpInfo("cumsum", core_ops.aten_cumsum, trace_only=True).xfail(
+        dtypes=(torch.int32,),
+        reason="fixme: torch.cumsum with int32 inputs uses int64 as the output type",
+    ),
     TorchLibOpInfo("contiguous", core_ops.aten_contiguous),
     TorchLibOpInfo(
         "ops.aten.convolution",
         core_ops.aten_convolution,
         trace_only=True,
         tolerance={torch.float32: (3.7e-5, 1.8e-4)},
     ),
@@ -1404,15 +1485,15 @@
     ),
     TorchLibOpInfo("native_batch_norm", core_ops.aten_native_batch_norm, trace_only=True),
     TorchLibOpInfo(
         "ops.aten.native_group_norm",
         core_ops.aten_native_group_norm,
         trace_only=True,
     ).xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: 'GroupNormKernelImpl' not implemented for 'Half' in nightly and weekly",
     ),
     TorchLibOpInfo(
         "native_layer_norm",
         core_ops.aten_native_layer_norm,
         trace_only=True,
         tolerance={torch.float32: (3.7e-5, 1.8e-4)},
@@ -1487,15 +1568,15 @@
         tolerance={torch.float32: (3.7e-5, 1.8e-4)},
     ),
     TorchLibOpInfo(
         "nn.functional.gelu",
         nn_ops.aten_gelu,
         trace_only=True,
     ).xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="fixme: ONNX Runtime aborted",
     ),
     TorchLibOpInfo("nn.functional.linear", nn_ops.aten_linear).skip(
         # input: input, args: weight, bias; so len(args) == 2 means bias is provided
         matcher=lambda sample: len(sample.args) != 1,
         reason="this overload is implemented for bias=None",
     ),
@@ -1627,14 +1708,20 @@
     )
     .xfail(
         matcher=lambda sample: "scale_factor" in sample.kwargs,
         reason="fixme: the scale_factor tests",
     ),
     TorchLibOpInfo("ones_like", core_ops.aten_ones_like, trace_only=True),
     TorchLibOpInfo(
+        "roll",
+        core_ops.aten_roll,
+        trace_only=True,
+        input_wrangler=_roll_input_wrangler,
+    ),
+    TorchLibOpInfo(
         "scatter_reduce",
         core_ops.aten_scatter_reduce,
         input_wrangler=_scatter_reduce_input_wrangler,
         trace_only=True,
     )
     .xfail(
         variant_name="mean",
@@ -1665,22 +1752,25 @@
     TorchLibOpInfo("slice", core_ops.aten_slice, trace_only=True),
     TorchLibOpInfo(
         "ops.aten.stft",  # Custom from extra_opinfo
         core_ops.aten_stft,
         trace_only=True,
         tolerance={torch.float32: (3.7e-5, 1.8e-4)},
     ).xfail(
-        dtypes=[torch.float16],
+        dtypes=(torch.float16,),
         reason="RuntimeError: MKL FFT doesn't support tensors of type: Half",
     ),
     TorchLibOpInfo(
         "sum",
         core_ops.aten_sum_dim_IntList,
         input_wrangler=_sum_input_wrangler,
         trace_only=True,
+    ).xfail(
+        dtypes=(torch.int32,),
+        reason="fixme: torch.sum uses int64 as the accumulator for int32 inputs",
     ),
     TorchLibOpInfo(
         "ops.aten.tensor.bool", core_ops.aten_tensor_bool
     ),  # Custom from extra_opinfo
     TorchLibOpInfo(
         "ops.aten.tensor.float", core_ops.aten_tensor_float  # Custom from extra_opinfo
     ),
@@ -1738,14 +1828,15 @@
 ops_test_common.duplicate_opinfo(OPS_DB, "arange", ("arange_start", "arange_start_step"))
 ops_test_common.duplicate_opinfo(OPS_DB, "argmax", ("argmax_dim",))
 ops_test_common.duplicate_opinfo(OPS_DB, "argmin", ("argmin_dim",))
 ops_test_common.duplicate_opinfo(OPS_DB, "atleast_1d", ("atleast_1d_single_tensor",))
 ops_test_common.duplicate_opinfo(OPS_DB, "atleast_2d", ("atleast_2d_single_tensor",))
 ops_test_common.duplicate_opinfo(OPS_DB, "atleast_3d", ("atleast_3d_single_tensor",))
 ops_test_common.duplicate_opinfo(OPS_DB, "cat", ("concat", "concatenate"))
+ops_test_common.duplicate_opinfo(OPS_DB, "clone", ("lift_fresh_copy",))
 ops_test_common.duplicate_opinfo(OPS_DB, "full_like", ("full_like_dtype",))
 ops_test_common.duplicate_opinfo(OPS_DB, "index_put", ("index_put_bool",))
 ops_test_common.duplicate_opinfo(OPS_DB, "max", ("max_dim",))
 ops_test_common.duplicate_opinfo(OPS_DB, "mean", ("mean_dim",))
 ops_test_common.duplicate_opinfo(OPS_DB, "min", ("min_dim",))
 ops_test_common.duplicate_opinfo(OPS_DB, "new_empty", ("new_empty_dtype",))
 ops_test_common.duplicate_opinfo(OPS_DB, "new_empty_strided", ("new_empty_strided_dtype",))
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/attr_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/attr_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/gemmgelu.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/gemmgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/gemmgelu_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/gemmgelu_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/if_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/if_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns1A_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/onnxfns1A_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns2_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/onnxfns2_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/onnxfns_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/ort_custom_ops.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/functions/ort_custom_ops.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/if_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/if_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/loop_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/loop_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/attrref.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/attrref.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/cast_like.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/cast_like.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/different_opset.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/different_opset.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/dropout.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/dropout.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/eager_op.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/eager_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/eg1.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/eg1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/getitem.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/getitem.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/graph_attr.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/graph_attr.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/identity.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/identity.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/if_statement.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/if_statement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/loops_break.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/loops_break.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/loops_while.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/loops_while.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns1.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/onnxfns1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns1A.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/onnxfns1A.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns2.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/onnxfns2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/opt_input.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/opt_input.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/opt_output.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/opt_output.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/renaming.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/renaming.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/sequences.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/sequences.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/signal_dft.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/signal_dft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/subfunction.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/subfunction.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/type_double.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/models/type_double.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/onnx_types_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/onnx_types_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/operator_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/tests/operator_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/type_annotation.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/type_annotation_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/type_annotation_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/utils.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/values.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript/values_test.py` & `onnxscript-preview-0.1.0.dev20230729/onnxscript/values_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/PKG-INFO` & `onnxscript-preview-0.1.0.dev20230729/onnxscript_preview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: onnxscript-preview
-Version: 0.1.0.dev20230726
-Summary: Authoring ONNX functions in Python
+Version: 0.1.0.dev20230729
+Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,26 +21,26 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Repository, https://github.com/onnx/onnxscript
+Project-URL: Repository, https://github.com/microsoft/onnxscript
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ----
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/SOURCES.txt` & `onnxscript-preview-0.1.0.dev20230729/onnxscript_preview.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 VERSION
 pyproject.toml
 setup.py
 onnxscript/__init__.py
 onnxscript/analysis.py
 onnxscript/analysis_test.py
-onnxscript/autocast.py
 onnxscript/converter.py
 onnxscript/converter_test.py
 onnxscript/evaluator.py
 onnxscript/evaluator_test.py
 onnxscript/irbuilder.py
 onnxscript/main.py
 onnxscript/onnx_types.py
@@ -23,15 +22,15 @@
 onnxscript/type_annotation.py
 onnxscript/type_annotation_test.py
 onnxscript/utils.py
 onnxscript/values.py
 onnxscript/values_test.py
 onnxscript/_internal/__init__.py
 onnxscript/_internal/ast_utils.py
-onnxscript/_internal/feature_switch.py
+onnxscript/_internal/autocast.py
 onnxscript/_internal/param_manipulation.py
 onnxscript/_internal/param_manipulation_test.py
 onnxscript/_internal/runtime_typing.py
 onnxscript/_internal/version_utils.py
 onnxscript/backend/__init__.py
 onnxscript/backend/onnx_backend.py
 onnxscript/backend/onnx_backend_test.py
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/pyproject.toml` & `onnxscript-preview-0.1.0.dev20230729/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onnxscript-preview"
 dynamic = ["version"]
-description = "Authoring ONNX functions in Python"
+description = "Naturally author ONNX functions and models using a subset of Python"
 authors = [{ name = "Microsoft Corporation", email = "onnx@microsoft.com" }]
-urls = { "Repository" = "https://github.com/onnx/onnxscript" }
+urls = { "Repository" = "https://github.com/microsoft/onnxscript" }
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Operating System :: POSIX",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "License :: OSI Approved :: Apache Software License",
+  "License :: OSI Approved :: MIT License",
 ]
 dependencies = ["numpy", "onnx>=1.14", "typing_extensions"]
 
 [tool.setuptools.packages.find]
 include = ["onnxscript*"]
 # Tests are by default excluded: https://setuptools.pypa.io/en/latest/userguide/package_discovery.html
```

### Comparing `onnxscript-preview-0.1.0.dev20230726/setup.py` & `onnxscript-preview-0.1.0.dev20230729/setup.py`

 * *Files identical despite different names*


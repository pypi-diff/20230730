# Comparing `tmp/mlpf-0.0.7.tar.gz` & `tmp/mlpf-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpf-0.0.7.tar", last modified: Sat Jun 24 21:34:24 2023, max compression
+gzip compressed data, was "mlpf-0.0.8.tar", last modified: Sun Jul 30 21:19:56 2023, max compression
```

## Comparing `mlpf-0.0.7.tar` & `mlpf-0.0.8.tar`

### file list

```diff
@@ -1,116 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.691975 mlpf-0.0.7/
--rw-rw-rw-   0        0        0      479 2023-06-24 21:27:28.000000 mlpf-0.0.7/CHANGELOG.md
--rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.7/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5038 2023-06-24 21:34:24.691975 mlpf-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4399 2023-06-24 21:34:11.000000 mlpf-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.442477 mlpf-0.0.7/examples/
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.442477 mlpf-0.0.7/examples/data/
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.473533 mlpf-0.0.7/examples/data/analysis/
--rw-rw-rw-   0        0        0     1390 2023-06-20 15:43:08.000000 mlpf-0.0.7/examples/data/analysis/describe_grid.py
--rw-rw-rw-   0        0        0     1238 2023-06-20 15:43:08.000000 mlpf-0.0.7/examples/data/analysis/describe_node.py
--rw-rw-rw-   0        0        0     1332 2023-06-20 15:43:08.000000 mlpf-0.0.7/examples/data/analysis/grid_pdf_estimates.py
--rw-rw-rw-   0        0        0     1249 2023-06-20 15:43:08.000000 mlpf-0.0.7/examples/data/analysis/node_pdf_estimates.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.478731 mlpf-0.0.7/examples/data/generate/
--rw-rw-rw-   0        0        0     1085 2023-06-20 15:43:08.000000 mlpf-0.0.7/examples/data/generate/uniform.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.442477 mlpf-0.0.7/examples/sklearn/
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.481970 mlpf-0.0.7/examples/sklearn/loss/
--rw-rw-rw-   0        0        0     1016 2023-06-24 10:31:44.000000 mlpf-0.0.7/examples/sklearn/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.486469 mlpf-0.0.7/examples/sklearn/supervised_power_flow/
--rw-rw-rw-   0        0        0     2985 2023-06-20 13:03:26.000000 mlpf-0.0.7/examples/sklearn/supervised_power_flow/linear_regression.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.443826 mlpf-0.0.7/examples/torch/
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.491469 mlpf-0.0.7/examples/torch/loss/
--rw-rw-rw-   0        0        0     1141 2023-06-24 10:31:11.000000 mlpf-0.0.7/examples/torch/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.492938 mlpf-0.0.7/examples/torch/supervised_power_flow/
--rw-rw-rw-   0        0        0     5501 2023-06-24 20:42:49.000000 mlpf-0.0.7/examples/torch/supervised_power_flow/gcn.py
--rw-rw-rw-   0        0        0     4639 2023-06-24 20:42:49.000000 mlpf-0.0.7/examples/torch/supervised_power_flow/mlp.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.492938 mlpf-0.0.7/examples/torch/unsupervised_power_flow/
--rw-rw-rw-   0        0        0     4961 2023-06-24 21:04:11.000000 mlpf-0.0.7/examples/torch/unsupervised_power_flow/gcn.py
--rw-rw-rw-   0        0        0     4048 2023-06-24 20:42:49.000000 mlpf-0.0.7/examples/torch/unsupervised_power_flow/mlp.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.494377 mlpf-0.0.7/mlpf/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.518549 mlpf-0.0.7/mlpf/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.526203 mlpf-0.0.7/mlpf/data/analysis/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.539489 mlpf-0.0.7/mlpf/data/analysis/description/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/analysis/description/__init__.py
--rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/analysis/description/describe.py
--rw-rw-rw-   0        0        0     1447 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/analysis/description/describe_grid.py
--rw-rw-rw-   0        0        0     1396 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/analysis/description/describe_node.py
--rw-rw-rw-   0        0        0     6433 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.556634 mlpf-0.0.7/mlpf/data/analysis/visualization/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/analysis/visualization/__init__.py
--rw-rw-rw-   0        0        0     3420 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/analysis/visualization/grid_pdf_estimates.py
--rw-rw-rw-   0        0        0     3473 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/analysis/visualization/node_pdf_estimates.py
--rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/analysis/visualization/visualize.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.562558 mlpf-0.0.7/mlpf/data/conversion/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.569287 mlpf-0.0.7/mlpf/data/conversion/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/numpy/__init__.py
--rw-rw-rw-   0        0        0     1788 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.574267 mlpf-0.0.7/mlpf/data/conversion/torch/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/torch/__init__.py
--rw-rw-rw-   0        0        0     1360 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/torch/power_flow.py
--rw-rw-rw-   0        0        0      475 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.574267 mlpf-0.0.7/mlpf/data/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.579303 mlpf-0.0.7/mlpf/data/data/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/data/numpy/__init__.py
--rw-rw-rw-   0        0        0     3922 2023-06-24 10:33:25.000000 mlpf-0.0.7/mlpf/data/data/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.584827 mlpf-0.0.7/mlpf/data/data/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/data/torch/__init__.py
--rw-rw-rw-   0        0        0     1584 2023-06-24 10:33:25.000000 mlpf-0.0.7/mlpf/data/data/torch/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.585826 mlpf-0.0.7/mlpf/data/generate/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/generate/__init__.py
--rw-rw-rw-   0        0        0     3523 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/generate/generate_uniform_data.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.591798 mlpf-0.0.7/mlpf/data/loading/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/loading/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/loading/load_data.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.605217 mlpf-0.0.7/mlpf/data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/utils/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/utils/masks.py
--rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/utils/pandapower_networks.py
--rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/utils/saving.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.634207 mlpf-0.0.7/mlpf/enumerations/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/__init__.py
--rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/branch_table.py
--rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/bus_table.py
--rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/bus_type.py
--rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/gencost_table.py
--rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/generator_table.py
--rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/power_flow_ids.py
--rw-rw-rw-   0        0        0     1254 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/enumerations/ppc_tables.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.639855 mlpf-0.0.7/mlpf/loss/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.654217 mlpf-0.0.7/mlpf/loss/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/numpy/__init__.py
--rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/numpy/bound_errors.py
--rw-rw-rw-   0        0        0     3828 2023-06-24 10:16:05.000000 mlpf-0.0.7/mlpf/loss/numpy/power_flow.py
--rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/numpy/utils.py
--rw-rw-rw-   0        0        0     1465 2023-06-24 10:16:05.000000 mlpf-0.0.7/mlpf/loss/relative_values.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.679814 mlpf-0.0.7/mlpf/loss/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/torch/__init__.py
--rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/torch/bound_errors.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.682241 mlpf-0.0.7/mlpf/loss/torch/metrics/
--rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.7/mlpf/loss/torch/metrics/__init__.py
--rw-rw-rw-   0        0        0     3615 2023-06-24 20:42:49.000000 mlpf-0.0.7/mlpf/loss/torch/metrics/active.py
--rw-rw-rw-   0        0        0     3711 2023-06-24 20:42:49.000000 mlpf-0.0.7/mlpf/loss/torch/metrics/reactive.py
--rw-rw-rw-   0        0        0      677 2023-06-24 10:16:05.000000 mlpf-0.0.7/mlpf/loss/torch/metrics/utils.py
--rw-rw-rw-   0        0        0     3202 2023-06-24 10:30:16.000000 mlpf-0.0.7/mlpf/loss/torch/power_flow.py
--rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/torch/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.687453 mlpf-0.0.7/mlpf/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/utils/__init__.py
--rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/utils/ppc.py
--rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/utils/standard_scaler.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.518549 mlpf-0.0.7/mlpf.egg-info/
--rw-rw-rw-   0        0        0     5038 2023-06-24 21:34:24.000000 mlpf-0.0.7/mlpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2633 2023-06-24 21:34:24.000000 mlpf-0.0.7/mlpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 21:34:24.000000 mlpf-0.0.7/mlpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-24 21:34:24.000000 mlpf-0.0.7/mlpf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-24 21:34:24.000000 mlpf-0.0.7/mlpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 21:34:24.691975 mlpf-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-06-24 21:33:08.000000 mlpf-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.690969 mlpf-0.0.7/test/
--rw-rw-rw-   0        0        0     2631 2023-06-24 10:16:05.000000 mlpf-0.0.7/test/test_power_flow_loss.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.750020 mlpf-0.0.8/
+-rw-rw-rw-   0        0        0      976 2023-07-30 21:12:48.000000 mlpf-0.0.8/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.8/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    13378 2023-07-30 21:19:56.750020 mlpf-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12723 2023-07-30 21:10:30.000000 mlpf-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.514799 mlpf-0.0.8/examples/
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.514799 mlpf-0.0.8/examples/data/
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.546132 mlpf-0.0.8/examples/data/analysis/
+-rw-rw-rw-   0        0        0     1390 2023-06-20 15:43:08.000000 mlpf-0.0.8/examples/data/analysis/describe_grid.py
+-rw-rw-rw-   0        0        0     1238 2023-06-20 15:43:08.000000 mlpf-0.0.8/examples/data/analysis/describe_node.py
+-rw-rw-rw-   0        0        0     2454 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/data/analysis/generator_overview.py
+-rw-rw-rw-   0        0        0     1332 2023-06-20 15:43:08.000000 mlpf-0.0.8/examples/data/analysis/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     1249 2023-06-20 15:43:08.000000 mlpf-0.0.8/examples/data/analysis/node_pdf_estimates.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.561750 mlpf-0.0.8/examples/data/generate/
+-rw-rw-rw-   0        0        0     1315 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/data/generate/uniform.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.514799 mlpf-0.0.8/examples/sklearn/
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.561750 mlpf-0.0.8/examples/sklearn/loss/
+-rw-rw-rw-   0        0        0     2549 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/sklearn/loss/optimal_power_flow.py
+-rw-rw-rw-   0        0        0     1156 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/sklearn/loss/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.514799 mlpf-0.0.8/examples/sklearn/supervised/
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.577333 mlpf-0.0.8/examples/sklearn/supervised/optimal_power_flow/
+-rw-rw-rw-   0        0        0     3102 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/sklearn/supervised/optimal_power_flow/linear_regression.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.577333 mlpf-0.0.8/examples/sklearn/supervised/power_flow/
+-rw-rw-rw-   0        0        0     2832 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/sklearn/supervised/power_flow/linear_regression.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.514799 mlpf-0.0.8/examples/torch/
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.577333 mlpf-0.0.8/examples/torch/loss/
+-rw-rw-rw-   0        0        0     2725 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/torch/loss/optimal_power_flow.py
+-rw-rw-rw-   0        0        0     1325 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/torch/loss/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.514799 mlpf-0.0.8/examples/torch/supervised/
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.577333 mlpf-0.0.8/examples/torch/supervised/optimal_power_flow/
+-rw-rw-rw-   0        0        0     6375 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/torch/supervised/optimal_power_flow/gcn.py
+-rw-rw-rw-   0        0        0     5626 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/torch/supervised/optimal_power_flow/mlp.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.577333 mlpf-0.0.8/examples/torch/supervised/power_flow/
+-rw-rw-rw-   0        0        0     5709 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/torch/supervised/power_flow/gcn.py
+-rw-rw-rw-   0        0        0     4853 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/torch/supervised/power_flow/mlp.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.514799 mlpf-0.0.8/examples/torch/unsupervised/
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.577333 mlpf-0.0.8/examples/torch/unsupervised/optimal_power_flow/
+-rw-rw-rw-   0        0        0     6426 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/torch/unsupervised/optimal_power_flow/gcn.py
+-rw-rw-rw-   0        0        0     5673 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/torch/unsupervised/optimal_power_flow/mlp.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.577333 mlpf-0.0.8/examples/torch/unsupervised/power_flow/
+-rw-rw-rw-   0        0        0     5169 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/torch/unsupervised/power_flow/gcn.py
+-rw-rw-rw-   0        0        0     4262 2023-07-30 21:10:30.000000 mlpf-0.0.8/examples/torch/unsupervised/power_flow/mlp.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.577333 mlpf-0.0.8/mlpf/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.613056 mlpf-0.0.8/mlpf/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.613056 mlpf-0.0.8/mlpf/data/analysis/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.624579 mlpf-0.0.8/mlpf/data/analysis/description/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/analysis/description/__init__.py
+-rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/analysis/description/describe.py
+-rw-rw-rw-   0        0        0     1447 2023-06-20 15:43:08.000000 mlpf-0.0.8/mlpf/data/analysis/description/describe_grid.py
+-rw-rw-rw-   0        0        0     1396 2023-06-20 15:43:08.000000 mlpf-0.0.8/mlpf/data/analysis/description/describe_node.py
+-rw-rw-rw-   0        0        0     6433 2023-06-20 15:43:08.000000 mlpf-0.0.8/mlpf/data/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.655838 mlpf-0.0.8/mlpf/data/analysis/visualization/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/analysis/visualization/__init__.py
+-rw-rw-rw-   0        0        0     3420 2023-06-20 15:43:08.000000 mlpf-0.0.8/mlpf/data/analysis/visualization/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     3473 2023-06-20 15:43:08.000000 mlpf-0.0.8/mlpf/data/analysis/visualization/node_pdf_estimates.py
+-rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/analysis/visualization/visualize.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.655838 mlpf-0.0.8/mlpf/data/conversion/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.8/mlpf/data/conversion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.655838 mlpf-0.0.8/mlpf/data/conversion/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.8/mlpf/data/conversion/numpy/__init__.py
+-rw-rw-rw-   0        0        0     5509 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/conversion/numpy/optimal_power_flow.py
+-rw-rw-rw-   0        0        0     2652 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/conversion/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.655838 mlpf-0.0.8/mlpf/data/conversion/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.8/mlpf/data/conversion/torch/__init__.py
+-rw-rw-rw-   0        0        0     3083 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/conversion/torch/optimal_power_flow.py
+-rw-rw-rw-   0        0        0     1996 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/conversion/torch/power_flow.py
+-rw-rw-rw-   0        0        0      475 2023-06-20 14:41:06.000000 mlpf-0.0.8/mlpf/data/conversion/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.655838 mlpf-0.0.8/mlpf/data/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/data/__init__.py
+-rw-rw-rw-   0        0        0     3698 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/data/optimal_power_flow.py
+-rw-rw-rw-   0        0        0     3263 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/data/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.671460 mlpf-0.0.8/mlpf/data/generate/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/generate/__init__.py
+-rw-rw-rw-   0        0        0     4067 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/generate/generate_uniform_data.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.671460 mlpf-0.0.8/mlpf/data/loading/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/loading/__init__.py
+-rw-rw-rw-   0        0        0     3947 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/loading/load_data.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.671460 mlpf-0.0.8/mlpf/data/masks/
+-rw-rw-rw-   0        0        0        0 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/masks/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/masks/optimal_power_flow.py
+-rw-rw-rw-   0        0        0     1439 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/data/masks/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.671460 mlpf-0.0.8/mlpf/data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/utils/__init__.py
+-rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/utils/pandapower_networks.py
+-rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/data/utils/saving.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.718763 mlpf-0.0.8/mlpf/enumerations/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/enumerations/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/enumerations/branch_table.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/enumerations/bus_table.py
+-rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/enumerations/bus_type.py
+-rw-rw-rw-   0        0        0      268 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/enumerations/gencost_table.py
+-rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/enumerations/generator_table.py
+-rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/enumerations/power_flow_ids.py
+-rw-rw-rw-   0        0        0     1254 2023-06-20 15:43:08.000000 mlpf-0.0.8/mlpf/enumerations/ppc_tables.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.718763 mlpf-0.0.8/mlpf/loss/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/loss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.718763 mlpf-0.0.8/mlpf/loss/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/loss/numpy/__init__.py
+-rw-rw-rw-   0        0        0     2290 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/bound_errors.py
+-rw-rw-rw-   0        0        0      892 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/costs.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.718763 mlpf-0.0.8/mlpf/loss/numpy/metrics/
+-rw-rw-rw-   0        0        0        0 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3037 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/metrics/active.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.734397 mlpf-0.0.8/mlpf/loss/numpy/metrics/bounds/
+-rw-rw-rw-   0        0        0        0 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/metrics/bounds/__init__.py
+-rw-rw-rw-   0        0        0     2121 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/metrics/bounds/active.py
+-rw-rw-rw-   0        0        0     2153 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/metrics/bounds/reactive.py
+-rw-rw-rw-   0        0        0     2085 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/metrics/bounds/voltage.py
+-rw-rw-rw-   0        0        0     2369 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/metrics/costs.py
+-rw-rw-rw-   0        0        0     1720 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/metrics/metrics.py
+-rw-rw-rw-   0        0        0     3077 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/metrics/reactive.py
+-rw-rw-rw-   0        0        0      797 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/metrics/utils.py
+-rw-rw-rw-   0        0        0     3910 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/numpy/power_flow.py
+-rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/loss/numpy/utils.py
+-rw-rw-rw-   0        0        0     1472 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/relative_values.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.734397 mlpf-0.0.8/mlpf/loss/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/loss/torch/__init__.py
+-rw-rw-rw-   0        0        0     2293 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/bound_errors.py
+-rw-rw-rw-   0        0        0      917 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/costs.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.734397 mlpf-0.0.8/mlpf/loss/torch/metrics/
+-rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.8/mlpf/loss/torch/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3740 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/metrics/active.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.734397 mlpf-0.0.8/mlpf/loss/torch/metrics/bounds/
+-rw-rw-rw-   0        0        0        0 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/metrics/bounds/__init__.py
+-rw-rw-rw-   0        0        0     2626 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/metrics/bounds/active.py
+-rw-rw-rw-   0        0        0     2658 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/metrics/bounds/reactive.py
+-rw-rw-rw-   0        0        0     2570 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/metrics/bounds/voltage.py
+-rw-rw-rw-   0        0        0     2734 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/metrics/costs.py
+-rw-rw-rw-   0        0        0     3836 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/metrics/reactive.py
+-rw-rw-rw-   0        0        0      678 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/metrics/utils.py
+-rw-rw-rw-   0        0        0     3268 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/loss/torch/power_flow.py
+-rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/loss/torch/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.734397 mlpf-0.0.8/mlpf/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.8/mlpf/utils/__init__.py
+-rw-rw-rw-   0        0        0      838 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/utils/ppc.py
+-rw-rw-rw-   0        0        0      683 2023-07-30 21:10:30.000000 mlpf-0.0.8/mlpf/utils/standard_scaler.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.608547 mlpf-0.0.8/mlpf.egg-info/
+-rw-rw-rw-   0        0        0    13378 2023-07-30 21:19:53.000000 mlpf-0.0.8/mlpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3827 2023-07-30 21:19:56.000000 mlpf-0.0.8/mlpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 21:19:53.000000 mlpf-0.0.8/mlpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-30 21:19:53.000000 mlpf-0.0.8/mlpf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-30 21:19:53.000000 mlpf-0.0.8/mlpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 21:19:56.750020 mlpf-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-07-30 21:19:22.000000 mlpf-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:19:56.750020 mlpf-0.0.8/test/
+-rw-rw-rw-   0        0        0     8429 2023-07-30 21:10:30.000000 mlpf-0.0.8/test/test_metrics.py
+-rw-rw-rw-   0        0        0     7325 2023-07-30 21:10:30.000000 mlpf-0.0.8/test/test_optimal_power_flow_loss.py
+-rw-rw-rw-   0        0        0     4410 2023-07-30 21:10:30.000000 mlpf-0.0.8/test/test_power_flow_loss.py
```

### Comparing `mlpf-0.0.7/LICENCE.txt` & `mlpf-0.0.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/examples/data/analysis/describe_grid.py` & `mlpf-0.0.8/examples/data/analysis/describe_grid.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/examples/data/analysis/describe_node.py` & `mlpf-0.0.8/examples/data/analysis/describe_node.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/examples/data/analysis/grid_pdf_estimates.py` & `mlpf-0.0.8/examples/data/analysis/grid_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/examples/data/analysis/node_pdf_estimates.py` & `mlpf-0.0.8/examples/data/analysis/node_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/examples/sklearn/loss/from_arrays.py` & `mlpf-0.0.8/examples/torch/loss/power_flow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 import copy
+import torch
 
-import numpy as np
 import pandapower as pp
 import pandapower.networks as pn
 
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 
-from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
-from mlpf.loss.numpy.power_flow import active_power_errors, reactive_power_errors
+from mlpf.data.conversion.torch.power_flow import (
+    extract_line_tensors,
+    extract_power_tensors,
+    extract_voltage_tensors
+)
+from mlpf.loss.torch.power_flow import (
+    active_power_errors,
+    reactive_power_errors
+)
 
 net = pn.case118()
 
 ppc = pp.converter.to_ppc(net, init="flat")
 
 ppopt = ppoption(OUT_ALL=0, VERBOSE=0)
 ppc, converged = runpf(copy.deepcopy(ppc), ppopt=ppopt)
 
-edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_arrays(ppc)
+# note: going from float64 to float32(the standard in torch) will increase the PF loss significantly
+active_powers, reactive_powers = extract_power_tensors(ppc, dtype=torch.float64)
+voltage_magnitudes, voltage_angles = extract_voltage_tensors(ppc, dtype=torch.float64)
+edge_index, conductances, susceptances = extract_line_tensors(ppc, dtype=torch.float64)
 
-active_errors = active_power_errors(edge_index, active_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
-reactive_errors = reactive_power_errors(edge_index, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+active_errors = active_power_errors(edge_index, active_powers, voltage_magnitudes, voltage_angles, conductances, susceptances)
+reactive_errors = reactive_power_errors(edge_index, reactive_powers, voltage_magnitudes, voltage_angles, conductances, susceptances)
 
-print(f"Total P loss = {np.sum(active_errors):.3e} p.u.")
-print(f"Total Q loss = {np.sum(reactive_errors):.3e} p.u.")
+print(f"Total P loss = {torch.sum(active_errors):.3e} p.u.")
+print(f"Total Q loss = {torch.sum(reactive_errors):.3e} p.u.")
```

### Comparing `mlpf-0.0.7/examples/torch/supervised_power_flow/gcn.py` & `mlpf-0.0.8/examples/torch/supervised/power_flow/gcn.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 from sklearn.model_selection import train_test_split
 from torch_geometric.loader import DataLoader
 from torchmetrics import MetricCollection, MeanSquaredError, R2Score
 from tqdm import tqdm
 
-from mlpf.data.data.torch.power_flow import power_flow_data
+from mlpf.data.data.power_flow import PowerFlowData
 from mlpf.data.generate.generate_uniform_data import generate_uniform_ppcs
 from mlpf.loss.torch.metrics.active import MeanActivePowerError, MeanRelativeActivePowerError
 from mlpf.loss.torch.metrics.reactive import MeanReactivePowerError, MeanRelativeReactivePowerError
 from mlpf.utils.standard_scaler import StandardScaler
 
 
 class GNN(torch.nn.Module):
@@ -25,15 +25,15 @@
         self.standard_scaler = standard_scaler
         self.graph_encoder = pyg.nn.GCN(in_channels=in_channels, hidden_channels=hidden_channels, num_layers=num_layers, out_channels=hidden_channels)
         self.linear = nn.Linear(in_features=hidden_channels, out_features=out_channels)
 
     def forward(self, data):
         out = self.standard_scaler(data.x)
         out = self.graph_encoder(x=out, edge_index=data.edge_index)
-        out = self.linear(out)[~data.feature_mask].reshape(data.target_vector.shape)
+        out = self.linear(out)[~data.PQVA_mask].reshape(data.target_vector.shape)
 
         return out
 
 
 def main():
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
@@ -60,18 +60,18 @@
         low=0.9,
         high=1.1
     )
 
     # ppc -> Data
     pf_data_list = []
     for solved_ppc in tqdm(solved_ppc_list, ascii=True, desc="Converting ppcs to data"):
-        pf_data_list.append(power_flow_data(solved_ppc))
+        pf_data_list.append(PowerFlowData(solved_ppc).to_pyg_data())
 
     for data in pf_data_list:
-        data.x[~data.feature_mask] = 0.0  # delete the target info from the input features
+        data.x[~data.PQVA_mask] = 0.0  # delete the target info from the input features
 
     data_train, data_val = train_test_split(pf_data_list, test_size=0.33, random_state=42)
 
     # Torch dataloaders
 
     train_loader = DataLoader(data_train, batch_size=batch_size, shuffle=True)
     val_loader = DataLoader(data_val, batch_size=batch_size, shuffle=False)
@@ -146,18 +146,21 @@
                 predictions = model(batch)
 
                 metrics_val(preds=predictions, target=output_scaler(batch.target_vector), power_flow_predictions=output_scaler.inverse(predictions), batch=batch)
 
         overall_metrics_train = metrics_train.compute()
         overall_metrics_val = metrics_val.compute()
 
+        # a nice progress bar
         description = "Training | Validation:"
-
         for key in overall_metrics_train.keys():
-            description += f" {key}: ({overall_metrics_train[key]:2.4f} | {overall_metrics_val[key]:2.4f});"
+            unit = getattr(metrics_train[key], 'unit', None)  # get metric unit if it exists
+            unit_brackets = f" [{unit}]" if unit is not None else ''
+
+            description += f" {key}{unit_brackets}: ({overall_metrics_train[key]:2.4f} | {overall_metrics_val[key]:2.4f});"
 
         progress_bar.set_description(description)
 
         metrics_train.reset()
         metrics_val.reset()
```

### Comparing `mlpf-0.0.7/examples/torch/supervised_power_flow/mlp.py` & `mlpf-0.0.8/examples/torch/supervised/power_flow/mlp.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 from sklearn.model_selection import train_test_split
 from torch_geometric.loader import DataLoader
 from torchmetrics import MetricCollection, MeanSquaredError, R2Score
 from tqdm import tqdm
 
-from mlpf.data.data.torch.power_flow import power_flow_data
+from mlpf.data.data.power_flow import PowerFlowData
 from mlpf.data.generate.generate_uniform_data import generate_uniform_ppcs
 from mlpf.loss.torch.metrics.active import MeanActivePowerError, MeanRelativeActivePowerError
 from mlpf.loss.torch.metrics.reactive import MeanReactivePowerError, MeanRelativeReactivePowerError
 from mlpf.utils.standard_scaler import StandardScaler
 
 
 def main():
@@ -43,15 +43,15 @@
         low=0.9,
         high=1.1
     )
 
     # ppc -> Data
     pf_data_list = []
     for solved_ppc in tqdm(solved_ppc_list, ascii=True, desc="Converting ppcs to data"):
-        pf_data_list.append(power_flow_data(solved_ppc))
+        pf_data_list.append(PowerFlowData(solved_ppc).to_pyg_data())
 
     data_train, data_val = train_test_split(pf_data_list, test_size=0.33, random_state=42)
 
     # Torch dataloaders
 
     train_loader = DataLoader(data_train, batch_size=batch_size, shuffle=True)
     val_loader = DataLoader(data_val, batch_size=batch_size, shuffle=False)
@@ -126,18 +126,21 @@
                 predictions = model(features)
 
                 metrics_val(preds=predictions, target=output_scaler(targets), power_flow_predictions=output_scaler.inverse(predictions), batch=batch)
 
         overall_metrics_train = metrics_train.compute()
         overall_metrics_val = metrics_val.compute()
 
+        # a nice progress bar
         description = "Training | Validation:"
-
         for key in overall_metrics_train.keys():
-            description += f" {key}: ({overall_metrics_train[key]:2.4f} | {overall_metrics_val[key]:2.4f});"
+            unit = getattr(metrics_train[key], 'unit', None)  # get metric unit if it exists
+            unit_brackets = f" [{unit}]" if unit is not None else ''
+
+            description += f" {key}{unit_brackets}: ({overall_metrics_train[key]:2.4f} | {overall_metrics_val[key]:2.4f});"
 
         progress_bar.set_description(description)
 
         metrics_train.reset()
         metrics_val.reset()
```

### Comparing `mlpf-0.0.7/examples/torch/unsupervised_power_flow/gcn.py` & `mlpf-0.0.8/examples/torch/unsupervised/power_flow/gcn.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 from sklearn.model_selection import train_test_split
 from torch_geometric.loader import DataLoader
 from torchmetrics import MetricCollection
 from tqdm import tqdm
 
-from mlpf.data.data.torch.power_flow import power_flow_data
+from mlpf.data.data.power_flow import PowerFlowData
 from mlpf.data.generate.generate_uniform_data import generate_uniform_ppcs
 from mlpf.loss.torch.metrics.active import MeanActivePowerError, MeanRelativeActivePowerError
 from mlpf.loss.torch.metrics.reactive import MeanReactivePowerError, MeanRelativeReactivePowerError
 from mlpf.utils.standard_scaler import StandardScaler
 
 
 class GNN(torch.nn.Module):
@@ -25,53 +25,53 @@
         self.standard_scaler = standard_scaler
         self.graph_encoder = pyg.nn.GCN(in_channels=in_channels, hidden_channels=hidden_channels, num_layers=num_layers, out_channels=hidden_channels)
         self.linear = nn.Linear(in_features=hidden_channels, out_features=out_channels)
 
     def forward(self, data):
         out = self.standard_scaler(data.x)
         out = self.graph_encoder(x=out, edge_index=data.edge_index)
-        out = self.linear(out)[~data.feature_mask].reshape(data.target_vector.shape)
+        out = self.linear(out)[~data.PQVA_mask].reshape(data.target_vector.shape)
 
         return out
 
 
 def main():
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     # Random seeds
     pyg.seed_everything(123)
 
     # Hyperparameters
-    num_epochs = 5000
+    num_epochs = 1000
     batch_size = 512
     hidden_channels = 100
     num_layers = 3
     learning_rate = 3e-4
 
     # Generate ppcs
 
     net = pn.case118()
     ppc = pp.converter.to_ppc(net, init="flat")
 
     base_ppc, converged = runpf(ppc, ppopt=ppoption(OUT_ALL=0, VERBOSE=0))
 
     solved_ppc_list = generate_uniform_ppcs(
         base_ppc,
-        how_many=1000,
+        how_many=5000,
         low=0.9,
         high=1.1
     )
 
     # ppc -> Data
     pf_data_list = []
     for solved_ppc in tqdm(solved_ppc_list, ascii=True, desc="Converting ppcs to data"):
-        pf_data_list.append(power_flow_data(solved_ppc))
+        pf_data_list.append(PowerFlowData(solved_ppc).to_pyg_data())
 
     for data in pf_data_list:
-        data.x[~data.feature_mask] = 0.0  # delete the target info from the input features
+        data.x[~data.PQVA_mask] = 0.0  # delete the target info from the input features
 
     data_train, data_val = train_test_split(pf_data_list, test_size=0.33, random_state=42)
 
     # Torch dataloaders
 
     train_loader = DataLoader(data_train, batch_size=batch_size, shuffle=True)
     val_loader = DataLoader(data_val, batch_size=batch_size, shuffle=False)
@@ -135,18 +135,21 @@
                 predictions = model(batch)
 
                 metrics_val(power_flow_predictions=predictions, batch=batch)
 
         overall_metrics_train = metrics_train.compute()
         overall_metrics_val = metrics_val.compute()
 
+        # a nice progress bar
         description = "Training | Validation:"
-
         for key in overall_metrics_train.keys():
-            description += f" {key}: ({overall_metrics_train[key]:2.4f} | {overall_metrics_val[key]:2.4f});"
+            unit = getattr(metrics_train[key], 'unit', None)  # get metric unit if it exists
+            unit_brackets = f" [{unit}]" if unit is not None else ''
+
+            description += f" {key}{unit_brackets}: ({overall_metrics_train[key]:2.4f} | {overall_metrics_val[key]:2.4f});"
 
         progress_bar.set_description(description)
 
         metrics_train.reset()
         metrics_val.reset()
```

### Comparing `mlpf-0.0.7/examples/torch/unsupervised_power_flow/mlp.py` & `mlpf-0.0.8/examples/torch/unsupervised/power_flow/mlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 from sklearn.model_selection import train_test_split
 from torch_geometric.loader import DataLoader
 from torchmetrics import MetricCollection
 from tqdm import tqdm
 
-from mlpf.data.data.torch.power_flow import power_flow_data
+from mlpf.data.data.power_flow import PowerFlowData
 from mlpf.data.generate.generate_uniform_data import generate_uniform_ppcs
 from mlpf.loss.torch.metrics.active import MeanActivePowerError, MeanRelativeActivePowerError
 from mlpf.loss.torch.metrics.reactive import MeanReactivePowerError, MeanRelativeReactivePowerError
 from mlpf.utils.standard_scaler import StandardScaler
 
 
 def main():
@@ -43,15 +43,15 @@
         low=0.9,
         high=1.1
     )
 
     # ppc -> Data
     pf_data_list = []
     for solved_ppc in tqdm(solved_ppc_list, ascii=True, desc="Converting ppcs to data"):
-        pf_data_list.append(power_flow_data(solved_ppc))
+        pf_data_list.append(PowerFlowData(solved_ppc).to_pyg_data())
 
     data_train, data_val = train_test_split(pf_data_list, test_size=0.33, random_state=42)
 
     # Torch dataloaders
 
     train_loader = DataLoader(data_train, batch_size=batch_size, shuffle=True)
     val_loader = DataLoader(data_val, batch_size=batch_size, shuffle=False)
@@ -115,18 +115,21 @@
                 predictions = model(batch.feature_vector)
 
                 metrics_val(power_flow_predictions=predictions, batch=batch)
 
         overall_metrics_train = metrics_train.compute()
         overall_metrics_val = metrics_val.compute()
 
+        # a nice progress bar
         description = "Training | Validation:"
-
         for key in overall_metrics_train.keys():
-            description += f" {key}: ({overall_metrics_train[key]:2.4f} | {overall_metrics_val[key]:2.4f});"
+            unit = getattr(metrics_train[key], 'unit', None)  # get metric unit if it exists
+            unit_brackets = f" [{unit}]" if unit is not None else ''
+
+            description += f" {key}{unit_brackets}: ({overall_metrics_train[key]:2.4f} | {overall_metrics_val[key]:2.4f});"
 
         progress_bar.set_description(description)
 
         metrics_train.reset()
         metrics_val.reset()
```

### Comparing `mlpf-0.0.7/mlpf/data/analysis/description/describe.py` & `mlpf-0.0.8/mlpf/data/analysis/description/describe.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/data/analysis/description/describe_grid.py` & `mlpf-0.0.8/mlpf/data/analysis/description/describe_grid.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/data/analysis/description/describe_node.py` & `mlpf-0.0.8/mlpf/data/analysis/description/describe_node.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/data/analysis/utils.py` & `mlpf-0.0.8/mlpf/data/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/data/analysis/visualization/grid_pdf_estimates.py` & `mlpf-0.0.8/mlpf/data/analysis/visualization/grid_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/data/analysis/visualization/node_pdf_estimates.py` & `mlpf-0.0.8/mlpf/data/analysis/visualization/node_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/data/analysis/visualization/visualize.py` & `mlpf-0.0.8/mlpf/data/analysis/visualization/visualize.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/data/data/numpy/power_flow.py` & `mlpf-0.0.8/test/test_power_flow_loss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,106 @@
-import copy
+import torch
+import unittest
+import warnings
 
 import numpy as np
+import pandapower as pp
+import pandapower.networks as pn
 
-from numpy import ndarray
-from types import SimpleNamespace
-from typing import Tuple
-
-from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
-from mlpf.data.utils.masks import create_feature_mask
-from mlpf.enumerations.bus_table import BusTableIds
-from mlpf.enumerations.power_flow_ids import PowerFlowFeatureIds
-from mlpf.loss.numpy.power_flow import active_power_errors, reactive_power_errors
-from mlpf.loss.relative_values import relative_values
-from mlpf.utils.ppc import ppc_runpf
+from pypower.ppoption import ppoption
+from pypower.runpf import runpf
+from typing import Dict
+from tqdm import tqdm
 
+from mlpf.data.conversion.numpy.power_flow import extract_power_arrays, extract_voltage_arrays, extract_line_arrays
+from mlpf.data.conversion.torch.power_flow import extract_power_tensors, extract_voltage_tensors, extract_line_tensors
+from mlpf.data.generate.generate_uniform_data import generate_uniform_ppcs
+from mlpf.data.utils.pandapower_networks import get_all_pandapower_networks
+
+from mlpf.loss.numpy import power_flow as pf_numpy
+from mlpf.loss.torch import power_flow as pf_torch
 
-def power_flow_data(ppc: dict, solve: bool = False, dtype: np.dtype = np.float64):
-    """
-    Extract all the relevant info from the ppc file as ndarrays and pack it into a PyG Data object.
 
-    :param ppc: PyPower case format object
-    :param solve: If True, a power flow calculation in PyPower will be called before extracting info.
-    :param dtype: Torch data type to cast the real valued tensors into.
+def torch_get_power_flow_loss(ppc: Dict, dtype: torch.dtype = torch.float64) -> float:
     """
-    if solve:
-        ppc = ppc_runpf(ppc)
+    Get power flow loss from a ppc.
 
-    edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_arrays(ppc, dtype=dtype)
+    :param ppc: pypower case format
+    :param dtype: torch data type
+    :return: loss
+    """
+    active_powers, reactive_powers = extract_power_tensors(ppc, dtype=dtype)
+    voltage_magnitudes, voltage_angles = extract_voltage_tensors(ppc, dtype=dtype)
+    edge_index, conductances, susceptances = extract_line_tensors(ppc, dtype=dtype)
 
-    PQVA_matrix = np.vstack((active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad)).T
-    feature_mask = create_feature_mask(ppc["bus"][:, BusTableIds.bus_type])
+    active_errors = pf_torch.active_power_errors(edge_index, active_powers, voltage_magnitudes, voltage_angles, conductances, susceptances)
+    reactive_errors = pf_torch.reactive_power_errors(edge_index, reactive_powers, voltage_magnitudes, voltage_angles, conductances, susceptances)
 
-    edge_attributes = np.vstack((conductances_pu, susceptances_pu))
-
-    return SimpleNamespace(
-        edge_index=edge_index,
-        x=PQVA_matrix,
-        edge_attr=edge_attributes,
-        PQVA_matrix=PQVA_matrix,
-        feature_mask=feature_mask,
-        conductances_pu=conductances_pu,
-        susceptances_pu=susceptances_pu,
-        feature_vector=PQVA_matrix[feature_mask],
-        target_vector=PQVA_matrix[~feature_mask]
-    )
+    return float(torch.sum(active_errors + reactive_errors))
 
 
-def get_relative_power_flow_errors(predictions: ndarray, data: SimpleNamespace) -> Tuple[ndarray, ...]:
+def numpy_get_power_flow_loss(ppc: Dict) -> float:
     """
-    Take model predictions and merge them with the corresponding data batch.
-    Calculate the relative power flow errors for the given predictions.
+    Get power flow loss from a ppc.
 
-    :param predictions: Power flow unknown variable predictions.
-    :param data: Data object from which the predictions came from.
-    :return: (relative active power errors, relative reactive power errors)
+    :param ppc: pypower case format
+    :return: loss
     """
-    PQVA_matrix_prediction = copy.deepcopy(data.PQVA_matrix)
-    PQVA_matrix_prediction[~data.feature_mask] = predictions.flatten()
+    active_powers, reactive_powers = extract_power_arrays(ppc, dtype=np.float64)
+    voltage_magnitudes, voltage_angles = extract_voltage_arrays(ppc, dtype=np.float64)
+    edge_index, conductances, susceptances = extract_line_arrays(ppc, dtype=np.float64)
+
+    active_errors = pf_numpy.active_power_errors(edge_index, active_powers, voltage_magnitudes, voltage_angles, conductances, susceptances)
+    reactive_errors = pf_numpy.reactive_power_errors(edge_index, reactive_powers, voltage_magnitudes, voltage_angles, conductances, susceptances)
+
+    return float(np.sum(active_errors + reactive_errors))
+
+
+class TestPowerFlowLoss(unittest.TestCase):
+    def test_many_topologies(self):
+        """
+        Test for various grids if the power flow loss function calculates the loss bellow a certain threshold for solved ppcs in float64 accuracy.
+        :return:
+        """
+        warnings.filterwarnings("ignore", message="Casting complex values to real discards the imaginary part")
+
+        nets = get_all_pandapower_networks()
+
+        tolerance_VA = 1  # P error + Q error on entire grid in Volt-Amps
+
+        for net in tqdm(nets, ascii=True, desc="Multiple topologies"):
+            ppc = pp.converter.to_ppc(net, init="flat")
+            ppc, converged = runpf(ppc, ppopt=ppoption(OUT_ALL=0, VERBOSE=0))
+
+            tolerance = tolerance_VA / ppc["baseMVA"]
+
+            self.assertLess(torch_get_power_flow_loss(ppc), tolerance)
+            self.assertLess(numpy_get_power_flow_loss(ppc), tolerance)
+
+    def test_case118_uniform(self):
+        """
+        Test for single topology but with random grid parameter values if the power flow loss function calculates the loss bellow a certain threshold for solved ppcs in float64 accuracy.
+        :return:
+        """
+        warnings.filterwarnings("ignore", message="Casting complex values to real discards the imaginary part")
+        net = pn.case118()
+        base_ppc = pp.converter.to_ppc(net, init="flat")
+
+        base_ppc, converged = runpf(base_ppc, ppopt=ppoption(OUT_ALL=0, VERBOSE=0))
 
-    active_powers = PQVA_matrix_prediction[:, PowerFlowFeatureIds.active_power]
-    reactive_powers = PQVA_matrix_prediction[:, PowerFlowFeatureIds.reactive_power]
+        ppc_list = generate_uniform_ppcs(
+            base_ppc,
+            how_many=1000,
+            low=0.9,
+            high=1.1
+        )
 
-    voltage_magnitudes = PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_magnitude]
-    angles_rad = PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_angle]
+        tolerance_VA = 1  # P error + Q error on entire grid in Volt-Amps
+        tolerance = tolerance_VA / base_ppc["baseMVA"]
 
-    active_errors = active_power_errors(edge_index=data.edge_index,
-                                        active_powers=active_powers,
-                                        voltages=voltage_magnitudes,
-                                        angles_rad=angles_rad,
-                                        conductances=data.conductances_pu,
-                                        susceptances=data.susceptances_pu)
-
-    reactive_errors = reactive_power_errors(edge_index=data.edge_index,
-                                            reactive_powers=reactive_powers,
-                                            voltages=voltage_magnitudes,
-                                            angles_rad=angles_rad,
-                                            conductances=data.conductances_pu,
-                                            susceptances=data.susceptances_pu)
+        for ppc in tqdm(ppc_list, ascii=True, desc="Single topology"):
+            self.assertLess(torch_get_power_flow_loss(ppc), tolerance)
+            self.assertLess(numpy_get_power_flow_loss(ppc), tolerance)
 
-    relative_active_power_errors = np.abs(relative_values(active_errors, active_powers))
-    relative_reactive_power_errors = np.abs(relative_values(reactive_errors, reactive_powers))
 
-    return relative_active_power_errors, relative_reactive_power_errors
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `mlpf-0.0.7/mlpf/data/generate/generate_uniform_data.py` & `mlpf-0.0.8/mlpf/data/generate/generate_uniform_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import copy
 import warnings
-from typing import Dict, List
 
 import numpy as np
+
 from numpy import ndarray
 from pypower.ppoption import ppoption
+from pypower.runopf import runopf
 from pypower.runpf import runpf
 from tqdm import tqdm
+from typing import Dict, List
 
 from mlpf.enumerations.bus_table import BusTableIds
 from mlpf.enumerations.generator_table import GeneratorTableIds
 
 
-def generate_uniform_ppcs(base_ppc: Dict, how_many: int, low: float = 0.9, high: float = 1.1) -> List[Dict]:
+def generate_uniform_ppcs(base_ppc: Dict, how_many: int, low: float = 0.9, high: float = 1.1, method: str = "pf") -> List[Dict]:
     """
     Generate a list of ppcs for which the values of bus[active power, reactive power, voltage magnitude, voltage angle]
-    and gen[active power, reactive power] is uniformly distributed around those same values in base_ppc. The ppcs come with a solved power flow.
+    and gen[active power, reactive power] are uniformly distributed around those same values in base_ppc. The ppcs come with a solved (optimal) power flow,
+    depending on the arguments.
 
     TODO add latex value~U(low*base_value, high*base_value)
 
 
     :param base_ppc: Base ppc around which to generate.
     :param how_many: How many ppcs to generate.
     :param low: Low value multiplier in the uniform distribution.
     :param high: High value multiplier in the uniform distribution.
-    :return: List of ppcs
+    :param method: "pf" or "opf". Default "pf".
+    :return: List of PPCs.
     """
     warnings.filterwarnings("ignore", message="Casting complex values to real discards the imaginary part")
 
     bus_variables = [BusTableIds.active_power_MW, BusTableIds.reactive_power_MVAr, BusTableIds.voltage_magnitude_pu, BusTableIds.voltage_angle_deg]
     gen_variables = [GeneratorTableIds.active_power_MW, GeneratorTableIds.reactive_power_MVAr]
 
     class UniformDistribution:
@@ -68,15 +72,24 @@
 
             for bus_variable in bus_variables:
                 random_ppc["bus"][:, bus_variable] = bus_distribution_parameters[bus_variable].sample(random_ppc["bus"].shape[0])
 
             for gen_variable in gen_variables:
                 random_ppc["gen"][:, gen_variable] = gen_distribution_parameters[gen_variable].sample(random_ppc["gen"].shape[0])
 
-            ppopt = ppoption(OUT_ALL=0, VERBOSE=0)
-            solved_random_ppc, converged = runpf(random_ppc, ppopt=ppopt)
+            if method == "pf":
+                ppopt = ppoption(OUT_ALL=0, VERBOSE=0)
+                solved_random_ppc, converged = runpf(random_ppc, ppopt=ppopt)
+
+            elif method == "opf":
+                ppopt = ppoption(OUT_ALL=0, VERBOSE=0)
+                solved_random_ppc = runopf(random_ppc, ppopt=ppopt)
+                converged = solved_random_ppc["success"]
+
+            else:
+                raise ValueError(f"Method '{method}' is not supported. Supported methods are 'pf' and 'opf'.")
 
         random_ppc_list.append(solved_random_ppc)
 
     return random_ppc_list
 
 # TODO test to see if the distribution really is uniform with the mean being the original value
```

### Comparing `mlpf-0.0.7/mlpf/data/loading/load_data.py` & `mlpf-0.0.8/mlpf/data/loading/load_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,27 @@
         data_sample = pickle.load(f)
 
     assert type(data_sample) == dict, "Data sample isn't a dictionary which is the expected type for PyPower case files"
 
     return data_sample
 
 
+def load_solved_from_tuple(filepath: str) -> Dict:
+    """
+    Load the solved PPC instance when the pickle file contains a tuple of (unsolved, solved).
+
+    :param filepath:
+    :return: Solved PPC.
+    """
+    with open(filepath, 'rb') as f:
+        unsolved_solved_tuple = pickle.load(f)
+
+    return unsolved_solved_tuple[1]
+
+
 def load_data(path: str,
               extension: str = ".p",
               load_sample_function: Callable = load_pickle_ppc,
               max_samples=None,
               shuffle=False) -> List[Any]:
     """
     Load all the data files with the given extension in the directory described by path. By default, assumes that the files are pickled.
```

### Comparing `mlpf-0.0.7/mlpf/data/utils/masks.py` & `mlpf-0.0.8/mlpf/data/masks/power_flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Final, List
-
 import numpy as np
+
 from numpy import ndarray
+from typing import Final, List
 
 from mlpf.enumerations.bus_type import BusTypeIds
 from mlpf.enumerations.power_flow_ids import PowerFlowFeatureIds
 
 
 class BusTypeMasks:
     """
@@ -13,15 +13,15 @@
     A True value specifies that the value is known.
     """
     Slack: Final[List[bool]] = [False, False, True, True]
     PQ: Final[List[bool]] = [True, True, False, False]
     PV: Final[List[bool]] = [True, False, True, False]
 
 
-def create_feature_mask(bus_types: ndarray) -> ndarray:
+def create_power_flow_feature_mask(bus_types: ndarray) -> ndarray:
     """
     Create a feature mask depending on the node types in the (active power, reactive power, voltage magnitude, voltage angle) format.
 
     :param bus_types: The bus types column from the bus table of the pypower case format.
     :return: Boolean feature mask.
     """
     feature_mask = np.zeros((len(bus_types), len(PowerFlowFeatureIds)), dtype=bool)
```

### Comparing `mlpf-0.0.7/mlpf/data/utils/pandapower_networks.py` & `mlpf-0.0.8/mlpf/data/utils/pandapower_networks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/data/utils/saving.py` & `mlpf-0.0.8/mlpf/data/utils/saving.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/enumerations/generator_table.py` & `mlpf-0.0.8/mlpf/enumerations/generator_table.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/enumerations/ppc_tables.py` & `mlpf-0.0.8/mlpf/enumerations/ppc_tables.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/loss/numpy/bound_errors.py` & `mlpf-0.0.8/mlpf/loss/numpy/bound_errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 
 from numpy import ndarray
 
 
-def upper_bound_error(value: ndarray, value_max: ndarray) -> ndarray:
+def upper_bound_errors(value: ndarray, value_max: ndarray) -> ndarray:
     """
     Return the difference between the value and its maximum value if the value is larger than the maximum value, otherwise return 0.
 
     :param value:  Value.
     :param value_max: Maximum allowed value.
     :return: Error.
     """
     return np.maximum(np.zeros_like(value), value - value_max)
 
 
-def lower_bound_error(value: ndarray, value_min: ndarray) -> ndarray:
+def lower_bound_errors(value: ndarray, value_min: ndarray) -> ndarray:
     """
     Return the difference between the value and its minimum value if the value is smaller than the minimum value, otherwise return 0.
 
     :param value: Value.
     :param value_min: Minimum allowed value.
     :return: Error.
     """
@@ -28,16 +28,16 @@
 def main():
     x = np.linspace(-5, 5, 1000)
     offset = 0
     values = (np.exp(-x ** 2) - 0.5) * 5 + offset
     upper_bound = np.cos(4 * x) + offset
     lower_bound = np.sin(4 * x) - 2 + offset
 
-    upper_error = upper_bound_error(values, upper_bound)
-    lower_error = lower_bound_error(values, lower_bound)
+    upper_error = upper_bound_errors(values, upper_bound)
+    lower_error = lower_bound_errors(values, lower_bound)
     upper_bound_mask = upper_error > 0
     lower_bound_mask = lower_error < 0
 
     alpha = 0.2
 
     fig, ax = plt.subplots(2, 1, sharex=True)
     fig.suptitle("NumPy - Upper and lower bound error demonstration")
```

### Comparing `mlpf-0.0.7/mlpf/loss/numpy/power_flow.py` & `mlpf-0.0.8/mlpf/loss/numpy/power_flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
 
 from numpy import ndarray
+from typing import Tuple
 
 
 def _scatter_sum(values: ndarray,
                  indices: ndarray,
-                 out_size: int):
+                 out_size: int) -> ndarray:
     """
     Same functionality as _torch_scatter.scatter_sum_.
 
     :param values: Array to be summed up.
     :param indices: Indices which define which elements will be summed together.
     :param out_size: Size(len) of the output array.
     :return: Resulting array.
@@ -18,15 +19,15 @@
     np.add.at(result, indices, values)
 
     return result
 
 
 def _equation_components(edge_index: ndarray,
                          voltages: ndarray,
-                         angles_rad: ndarray):
+                         angles_rad: ndarray) -> Tuple[ndarray, ...]:
     """
     Extract the values used in the power flow equations.
 
     :param edge_index:
     :param voltages:
     :param angles_rad:
     :return:
@@ -45,15 +46,15 @@
 
 
 def active_power_errors(edge_index: ndarray,
                         active_powers: ndarray,
                         voltages: ndarray,
                         angles_rad: ndarray,
                         conductances: ndarray,
-                        susceptances: ndarray):
+                        susceptances: ndarray) -> ndarray:
     """
     Active power error as defined by the power flow equations.
 
     TODO Latex
 
     :param edge_index: Edge list.
     :param active_powers: Active powers.
@@ -76,15 +77,15 @@
 
 
 def reactive_power_errors(edge_index: ndarray,
                           reactive_powers: ndarray,
                           voltages: ndarray,
                           angles_rad: ndarray,
                           conductances: ndarray,
-                          susceptances: ndarray):
+                          susceptances: ndarray) -> ndarray:
     """
     Reactive power error as defined by the power flow equations.
 
     TODO Latex
 
     :param edge_index: Edge list.
     :param reactive_powers: Active powers.
```

### Comparing `mlpf-0.0.7/mlpf/loss/numpy/utils.py` & `mlpf-0.0.8/mlpf/loss/numpy/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/loss/relative_values.py` & `mlpf-0.0.8/mlpf/loss/relative_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import torch
 from numpy import ndarray
 from torch import Tensor
 
 
-def relative_values(numerator: Any, denominator: Any, eps: float = 1e-9, fill: bool = True):
+def relative_values(numerator: Any, denominator: Any, eps: float = 1e-9, fill: bool = True) -> Any:
     # TODO test for arrays and tensors. What happens when fill=False and denominator is all zeros
     """
     Return the relative value of the numerator with respect to the denominator, all while protecting against
     divisions by zero or close to zero values.
 
     :param numerator: Array/Tensor to be divided.
     :param denominator: Array/Tensor to divide with.
```

### Comparing `mlpf-0.0.7/mlpf/loss/torch/bound_errors.py` & `mlpf-0.0.8/mlpf/loss/torch/bound_errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import torch
 
 from torch import Tensor
 
 
-def upper_bound_error(value: Tensor, value_max: Tensor) -> Tensor:
+def upper_bound_errors(value: Tensor, value_max: Tensor) -> Tensor:
     """
     Return the difference between the value and its maximum value if the value is larger than the maximum value, otherwise return 0.
 
     :param value:  Value.
     :param value_max: Maximum allowed value.
     :return: Error.
     """
     return torch.maximum(torch.zeros_like(value), value - value_max)
 
 
-def lower_bound_error(value: Tensor, value_min: Tensor) -> Tensor:
+def lower_bound_errors(value: Tensor, value_min: Tensor) -> Tensor:
     """
     Return the difference between the value and its minimum value if the value is smaller than the minimum value, otherwise return 0.
 
     :param value: Value.
     :param value_min: Minimum allowed value.
     :return: Error.
     """
@@ -28,16 +28,16 @@
 def main():
     x = torch.linspace(-5, 5, 1000)
     offset = 0
     values = (torch.exp(-x ** 2) - 0.5) * 5 + offset
     upper_bound = torch.cos(x) + offset
     lower_bound = torch.sin(x) - 2 + offset
 
-    upper_error = upper_bound_error(values, upper_bound)
-    lower_error = lower_bound_error(values, lower_bound)
+    upper_error = upper_bound_errors(values, upper_bound)
+    lower_error = lower_bound_errors(values, lower_bound)
     upper_bound_mask = upper_error > 0
     lower_bound_mask = lower_error < 0
 
     alpha = 0.2
 
     fig, ax = plt.subplots(2, 1, sharex=True)
     fig.suptitle("Torch - Upper and lower bound error demonstration")
```

### Comparing `mlpf-0.0.7/mlpf/loss/torch/metrics/active.py` & `mlpf-0.0.8/mlpf/loss/torch/metrics/active.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,23 +29,27 @@
     def update(self, power_flow_predictions: Tensor, batch: Data):
         self.PQVA_matrix_prediction = incorporate_predictions(power_flow_predictions, batch)
 
         self.active_errors = active_power_errors(edge_index=batch.edge_index,
                                                  active_powers=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.active_power],
                                                  voltages=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_magnitude],
                                                  angles_rad=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_angle],
-                                                 conductances=batch.conductances_pu,
-                                                 susceptances=batch.susceptances_pu)
+                                                 conductances=batch.conductances,
+                                                 susceptances=batch.susceptances)
 
         self.active_error_sum += torch.sum(torch.abs(self.active_errors))
         self.node_count += self.active_errors.shape[0]
 
     def compute(self) -> Tensor:
         return self.active_error_sum / self.node_count
 
+    @property
+    def unit(self) -> str:
+        return "p.u."
+
 
 class MeanRelativeActivePowerError(Metric):
     """
     A TorchMetric class for calculating the average relative absolute active power flow error.
 
     TODO Latex
     """
@@ -62,15 +66,19 @@
     def update(self, power_flow_predictions: Tensor, batch: Data):
         self.PQVA_matrix_prediction = incorporate_predictions(power_flow_predictions, batch)
 
         self.active_errors = active_power_errors(edge_index=batch.edge_index,
                                                  active_powers=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.active_power],
                                                  voltages=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_magnitude],
                                                  angles_rad=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_angle],
-                                                 conductances=batch.conductances_pu,
-                                                 susceptances=batch.susceptances_pu)
+                                                 conductances=batch.conductances,
+                                                 susceptances=batch.susceptances)
 
         self.relative_active_error_sum += torch.sum(torch.abs(relative_values(self.active_errors, self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.active_power])))
         self.node_count += self.active_errors.shape[0]
 
     def compute(self) -> Tensor:
         return self.relative_active_error_sum / self.node_count
+
+    @property
+    def unit(self) -> str:
+        return "ratio"
```

### Comparing `mlpf-0.0.7/mlpf/loss/torch/metrics/reactive.py` & `mlpf-0.0.8/mlpf/loss/torch/metrics/reactive.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,23 +29,27 @@
     def update(self, power_flow_predictions: Tensor, batch: Data):
         self.PQVA_matrix_prediction = incorporate_predictions(power_flow_predictions, batch)
 
         self.reactive_errors = reactive_power_errors(edge_index=batch.edge_index,
                                                      reactive_powers=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.reactive_power],
                                                      voltages=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_magnitude],
                                                      angles_rad=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_angle],
-                                                     conductances=batch.conductances_pu,
-                                                     susceptances=batch.susceptances_pu)
+                                                     conductances=batch.conductances,
+                                                     susceptances=batch.susceptances)
 
         self.reactive_error_sum += torch.sum(torch.abs(self.reactive_errors))
         self.node_count += self.reactive_errors.shape[0]
 
     def compute(self) -> Tensor:
         return self.reactive_error_sum / self.node_count
 
+    @property
+    def unit(self) -> str:
+        return "p.u."
+
 
 class MeanRelativeReactivePowerError(Metric):
     """
     A TorchMetric class for calculating the average relative absolute reactive power flow error.
 
     TODO Latex
     """
@@ -62,15 +66,19 @@
     def update(self, power_flow_predictions: Tensor, batch: Data):
         self.PQVA_matrix_prediction = incorporate_predictions(power_flow_predictions, batch)
 
         self.reactive_errors = reactive_power_errors(edge_index=batch.edge_index,
                                                      reactive_powers=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.reactive_power],
                                                      voltages=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_magnitude],
                                                      angles_rad=self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_angle],
-                                                     conductances=batch.conductances_pu,
-                                                     susceptances=batch.susceptances_pu)
+                                                     conductances=batch.conductances,
+                                                     susceptances=batch.susceptances)
 
         self.relative_reactive_error_sum += torch.sum(torch.abs(relative_values(self.reactive_errors, self.PQVA_matrix_prediction[:, PowerFlowFeatureIds.reactive_power])))
         self.node_count += self.reactive_errors.shape[0]
 
     def compute(self) -> Tensor:
         return self.relative_reactive_error_sum / self.node_count
+
+    @property
+    def unit(self) -> str:
+        return "ratio"
```

### Comparing `mlpf-0.0.7/mlpf/loss/torch/power_flow.py` & `mlpf-0.0.8/mlpf/loss/torch/power_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import torch
 
 from torch import Tensor
-
 from torch_scatter import scatter_sum
+from typing import Tuple
 
 
 def _equation_components(edge_index: Tensor,
                          voltages: Tensor,
-                         angles_rad: Tensor):
+                         angles_rad: Tensor) -> Tuple[Tensor, ...]:
     """
     Extract the values used in the power flow equations.
 
     :param edge_index:
     :param voltages:
     :param angles_rad:
     :return:
@@ -30,15 +30,15 @@
 
 
 def active_power_errors(edge_index: Tensor,
                         active_powers: Tensor,
                         voltages: Tensor,
                         angles_rad: Tensor,
                         conductances: Tensor,
-                        susceptances: Tensor):
+                        susceptances: Tensor) -> Tensor:
     """
     Active power error as defined by the power flow equations.
 
     TODO Latex
 
     :param edge_index: Edge list.
     :param active_powers: Active powers.
@@ -60,15 +60,15 @@
 
 
 def reactive_power_errors(edge_index: Tensor,
                           reactive_powers: Tensor,
                           voltages: Tensor,
                           angles_rad: Tensor,
                           conductances: Tensor,
-                          susceptances: Tensor):
+                          susceptances: Tensor) -> Tensor:
     """
     Reactive power error as defined by the power flow equations.
 
     TODO Latex
 
     :param edge_index: Edge list.
     :param reactive_powers: Active powers.
```

### Comparing `mlpf-0.0.7/mlpf/loss/torch/utils.py` & `mlpf-0.0.8/mlpf/loss/torch/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.7/mlpf/utils/standard_scaler.py` & `mlpf-0.0.8/mlpf/utils/standard_scaler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import torch
-from torch import nn
+from torch import nn, Tensor
 
 
 class StandardScaler(nn.Module):
     """
     Standard scaler transform as a torch module.
     """
 
     def __init__(self, X):
         super(StandardScaler, self).__init__()
 
         self.mean = torch.mean(X, dim=0)
         self.std = torch.std(X, dim=0)
         self.std[self.std < 1e-9] = 1.0
 
-    def forward(self, x):
+    def forward(self, x) -> Tensor:
         return (x - self.mean) / self.std
 
     def _apply(self, fn):
         super(StandardScaler, self)._apply(fn)
         self.mean = fn(self.mean)
         self.std = fn(self.std)
 
         return self
 
-    def inverse(self, z):
+    def inverse(self, z) -> Tensor:
         return z * self.std + self.mean
```

### Comparing `mlpf-0.0.7/setup.py` & `mlpf-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
     'Topic :: Scientific/Engineering :: Artificial Intelligence'
 ]
 
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+long_description = (this_directory / "README.md").read_text(errors="ignore")
 
 setup(
     name='mlpf',
-    version='0.0.7',
+    version='0.0.8',
     description='Machine learning for power flow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     author='Viktor Todosijevic',
     author_email='todosijevicviktor998@gmail.com',
     license='MIT',
     classifiers=classifiers,
-    keywords=['machine learning', 'power flow', 'optimal power flow'],
+    keywords=['machine learning', 'power flow'],
     packages=find_packages(),
     install_requires=['numpy', 'pandapower', 'PYPOWER', 'scikit-learn', 'scipy', 'tqdm']
 )
```

